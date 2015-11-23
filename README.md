netuitive.packages.linux 1.0.0
----------------------

**Default Collectors**
The following are the collectors that are enabled by default in the Netuitive Agent, and are the ones we assume Diamond customers will use by default as well.

 - **CPU** - collects CPU utilization metric using /proc/stat
 - **DiskSpace** - uses /proc/mounts and os.statvfs() to get disk space usage
 - **DiskUsage** - collects I/O statistics from disks using /proc/diskstats
 - **LoadAverage** - uses /proc/loadavg to collect data on load average
 - **Memory** - collects data on memory utilization
 - **Network** - collects metrics on network interface usage using /proc/net/dev 
 - **VMStat** - uses /proc/vmstat to collect data
   on virtual memory manager
