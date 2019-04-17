# netuitive.packages.linux

For detailed information on this package, please refer to the [online documentation](https://help.netuitive.com/Content/Integrations/linux.htm).

## Default Collectors
The following are the collectors that are enabled by default in the Netuitive Agent, and are the ones we assume Netuitive customers will use by default as well.

 - **CPU** - collects CPU utilization metric using /proc/stat
 - **DiskSpace** - uses /proc/mounts and os.statvfs() to get disk space usage
 - **DiskUsage** - collects I/O statistics from disks using /proc/diskstats
 - **Heartbeat** - sends a metric with a value of 1 on every collection cycle
 - **LoadAverage** - uses /proc/loadavg to collect data on load average
 - **Memory** - collects data on memory utilization
 - **Network** - collects metrics on network interface usage using /proc/net/dev
 - **VMStat** - uses /proc/vmstat to collect data
   on virtual memory manager

Additional collectors may be enabled; policies and configurations for those collectors will be package separately as they become available.