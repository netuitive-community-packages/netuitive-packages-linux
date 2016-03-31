#netuitive.packages.linux 2.3.0

For detailed information on this package, please refer to the [online documentation](https://help.app.netuitive.com/Content/Misc/Datasources/Netuitive/new_netuitive_datasource.htm).

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

###Version 2.3.0

* Updated configurations so that EC2 elements which are also receiving Linux metrics from the Netuitive agent will be able to handle those metrics correctly.
* Removed two obsolete computed metrics.

###Version 2.2.0

* Added new policy: "Linux - Heavy CPU Load"
* Added new policy: "Linux - Heavy Disk Load"
* Added new policy: "Linux - Heavy Disk Load with Slow Performance"
* Added new policy: "Linux - Memory Utilization Exceeded"
* Fixed a bug in policy "Linux - Disk Utilization Threshold Exceeded" where the wrong metric was being evaluated.
* Added new computed metrics to summarize activity across all disks.
* Updated the "Linux Summary" dashboard to display graphs of the highest disk activity.

###Version 2.1.0

* Added Linux-specific element detail page.
* Updated memory percent and network error percent metrics to show as percentages.

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
