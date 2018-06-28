{
    "datacenter": "dc1",                // 数据中心名称
    "data_dir": "/var/lib/consul",      // Server 节点数据目录
    "log_level": "INFO",                // 日志级别
    "node_name": "docker1.node",        // 当前节点名称
    "server": true,                     // 是否为 Server 模式，false 为 Client 模式
    "ui": true,                         // 是否开启 UI 访问
    "bootstrap_expect": 1,              // 启动时期望的就绪节点，1 代表启动为 bootstrap 模式，等待其他节点加入
    "bind_addr": "192.168.1.11",        // 绑定的 IP
    "client_addr": "192.168.1.11",      // 同时作为 Client 接受请求的绑定 IP
    "retry_join": ["192.168.1.12","192.168.1.13"],  // 尝试加入的其他节点
    "retry_interval": "3s",             // 每次尝试间隔
    "raft_protocol": 3,                 // Raft 协议版本
    "enable_debug": false,              // 是否开启 Debug 模式
    "rejoin_after_leave": true,         // 允许重新加入集群
    "enable_syslog": false              // 是否开启 syslog
}
