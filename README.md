# V2Ray-VPN instruction
由于GFW对SS/SSR端口封锁加剧，想自己搭梯子的可参考V2Ray。  V2Ray使用了新的自行研发的VMess协议，改正了SS一些缺点，使用动态端口可改变通信的端口，对抗对长时间大流量端口的限速封锁，所以更难被墙检测到。

## 前提条件

1. 需要租用一台境外VPS。

2. 下载V2Ray客户端
    ### Windows: 
    V2RayN: https://github.com/2dust/v2rayN/releases  
    V2RayW: https://github.com/Cenmrev/V2RayW/releases  
    V2RayS: https://github.com/Shinlor/V2RayS/releases  
    Clash: https://github.com/Fndroid/clash_for_windows_pkg/releases  
    Windows系统建议使用V2rayN
    ### Mac:
    V2RayU: https://github.com/yanue/V2rayU/releases  
    V2RayX: https://github.com/Cenmrev/V2RayX/releases  
    ClashX: https://github.com/yichengchen/clashX/releases  
    Mac OS X系统建议使用V2rayU
    ### Android:
    V2RayNG: https://github.com/yanue/V2rayU/releases  
    ### 暂无免费IOS端

## 搭建V2Ray
1. 远程服务器  
   我是用putty链接的
2. 安装wget  
   ubuntu为例 `apt-get update && apt-get install wget`  
3. 下载安装V2Ray  
   `wget https://install.direct/go.sh`  
   `bash go.sh`  
4. 启动服务  
   `systemctl start v2ray'  
5. 配置文件  
   `/etc/v2ray/config.json`  
   获取id，端口号(port)和alterId, 或者修改成自己设置的然后重启服务  
   重启：`systemctl restart v2ray`  
   停止：`systemctl stop v2ray`  
   开机自启：`systemctl enable v2ray`  
6. 防火墙  
   开放对应端口的防火墙
   
## 配置客户端
1. 添加VMess服务器  
2. 填写服务端配置文件中对应的信息即可  
3. 两种模式PAC和全局  
    PAC：国内本地网络依然走本地路线，国外网站走代理路线  
    全局：不管国内国外，统一走代理路线
    
## Google TCP BBR加速器（可选）
1. 下载  
`wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh`  
2. 修改权限  
`chmod +x bbr.sh`  
3. 启动  
`./bbr.sh`

