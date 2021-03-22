# adj-monitoring-stack
To Monitoring the servers which act as a load balancer and terminate TLS

# Architectural Diagram for problem statement
- SSL Offloading
- SSL offloading with a reverse proxy

### SSL Offloading
![with out proxy](/images/Architecture_Solution_Diagram_without_proxy.png)

### SSL offloading with a reverse proxy
![with proxy](/images/Architecture_Solution_Diagram.png)

# Which Metrics To Monitor ?

* Server Stats
* Proxy Server Stats
* Network Stat Dump
* Linux Kernel Dump
* Process Monitoring Metrics

### Server Stats

 Type | Description
------------ | -------------
CPU Stats    | To monitor CPU metrics (user,system,io,nice)
Disk Stats	 | Get the Metrics from /proc/diskstats
FileSystem Stats | Storage system used
loadavg 	 | Get the Metrics from /proc/loadavg to identify the workload for the last 15min
netstat	 | Active Internet connections (only servers)
meminfo 	 | Memory related metrics of server to identify memory issues
filefd	 | Exposes file descriptor statistics from /proc/sys/fs/file-nr 

