# V2Ray-VPN instruction
由于GFW对SS/SSR端口封锁加剧，想自己搭梯子的可参考V2Ray。  V2Ray使用了新的自行研发的VMess协议，改正了SS一些缺点，使用动态端口可改变通信的端口，对抗对长时间大流量端口的限速封锁，所以更难被墙检测到。

## 前提条件

1. 需要租用一台境外VPS。

2. 下载putty客户端 https://www.putty.org/

3. 下载V2Ray客户端
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

1. 安装wget  
   `apt-get update && apt-get install wget`  
2. 下载安装V2Ray  
   `wget https://install.direct/go.sh`  
   `bash go.sh`  
3. 

