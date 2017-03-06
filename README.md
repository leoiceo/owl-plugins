# owl-plugins

* proc_resource_status 【进程监控】

```
[
    {
        "metric": "process.cpu.user", 
        "value": 3334, 
        "data_type": "counter", 
        "tags": {
            "proname": "nginx"
        }
    }, 
    {
        "metric": "process.fd", 
        "value": 64, 
        "data_type": "gauge", 
        "tags": {
            "proname": "nginx"
        }
    }, 
    {
        "metric": "process.cpu.sys", 
        "value": 1063, 
        "data_type": "counter", 
        "tags": {
            "proname": "nginx"
        }
    }, 
    {
        "metric": "process.swap", 
        "value": 0, 
        "data_type": "gauge", 
        "tags": {
            "proname": "nginx"
        }
    }, 
    {
        "metric": "process.cpu.all", 
        "value": 4397, 
        "data_type": "counter", 
        "tags": {
            "proname": "nginx"
        }
    }, 
    {
        "metric": "process.mem", 
        "value": 2981888, 
        "data_type": "gauge", 
        "tags": {
            "proname": "nginx"
        }
    }
]

```
* check_connections 【连接数据监控】
```
[
    {
        "metric": "ss.tcp_closing", 
        "data_type": "gauge", 
        "value": 0
    }, 
    {
        "metric": "ss.tcp_listen", 
        "data_type": "gauge", 
        "value": 13
    }, 
    {
        "metric": "ss.tcp_syn_sent", 
        "data_type": "gauge", 
        "value": 0
    }, 
    {
        "metric": "ss.tcp_syn_recv", 
        "data_type": "gauge", 
        "value": 0
    }, 
    {
        "metric": "ss.error_status", 
        "data_type": "gauge", 
        "value": 0
    }, 
    {
        "metric": "ss.tcp_established", 
        "data_type": "gauge", 
        "value": 64
    }, 
    {
        "metric": "ss.tcp_time_wait", 
        "data_type": "gauge", 
        "value": 3
    }, 
    {
        "metric": "ss.tcp_close", 
        "data_type": "gauge", 
        "value": 0
    }, 
    {
        "metric": "ss.tcp_fin_wait1", 
        "data_type": "gauge", 
        "value": 0
    }, 
    {
        "metric": "ss.tcp_fin_wait2", 
        "data_type": "gauge", 
        "value": 0
    }, 
    {
        "metric": "ss.tcp_close_wait", 
        "data_type": "gauge", 
        "value": 0
    }, 
    {
        "metric": "ss.tcp_last_ack", 
        "data_type": "gauge", 
        "value": 0
    }
]

```
* check_port 【端口监控】
eg: check_port 80,10100
```
[
    {
        "metric": "net.port.listen", 
        "value": 1, 
        "data_type": "gauge", 
        "tags": {
            "port": "80"
        }
    }, 
    {
        "metric": "net.port.listen", 
        "value": 3, 
        "data_type": "gauge", 
        "tags": {
            "port": "10100"
        }
    }
]

```
* check_url 【站点监控】
eg: check_url www.qq.com
```
[
    {
        "metric": "url.http_namelookup_time", 
        "value": 0.001, 
        "data_type": "GAUGE", 
        "tags": {
            "check_url": "www.qq.com"
        }
    }, 
    {
        "metric": "url.http_total_time", 
        "value": 0.035999999999999997, 
        "data_type": "GAUGE", 
        "tags": {
            "check_url": "www.qq.com"
        }
    }, 
    {
        "metric": "url.http_code", 
        "value": 200.0, 
        "data_type": "GAUGE", 
        "tags": {
            "check_url": "www.qq.com"
        }
    }, 
    {
        "metric": "url.http_conn_time", 
        "value": 0.01, 
        "data_type": "GAUGE", 
        "tags": {
            "check_url": "www.qq.com"
        }
    }
]
```
