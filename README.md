#netuitive.packages.linux 2.0.1

##Default Collectors
The following are the collectors that are enabled by default in the Netuitive Agent, and are the ones we assume Netuitive customers will use by default as well.

 - **CPU** - collects CPU utilization metric using /proc/stat
 - **DiskSpace** - uses /proc/mounts and os.statvfs() to get disk space usage
 - **DiskUsage** - collects I/O statistics from disks using /proc/diskstats
 - **LoadAverage** - uses /proc/loadavg to collect data on load average
 - **Memory** - collects data on memory utilization
 - **Network** - collects metrics on network interface usage using /proc/net/dev 
 - **VMStat** - uses /proc/vmstat to collect data
   on virtual memory manager

Additional collectors may be enabled; policies and configurations for those collectors will be package separately as they become available.

##Release History

###Version 2.0.1

* Fixed bug where some widgets on the summary dashboard were referencing old metric names.

###Version 2.0.0

* Added units to all metrics.
* Added new policy: "Linux - CPU Threshold Exceeded"
* Added new policy: "Linux - Disk Utilization Threshold Exceeded"
* Updated computed metric names for new naming convention

###Version 1.1.0

* Added summary dashboard.

###Version 1.0.0

* Initial production release of the package for monitoring Linux OS resources.
