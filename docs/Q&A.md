Q1:VM 克隆虚拟机 网卡启动失败
Err Msg: Failed to start LSB: Bring up/down networking
A1:# 依次执行以下指令
    systemctl stop NetworkManager
    systemctl disable NetworkManager
    #重新启动网络：
    systemctl start network.service