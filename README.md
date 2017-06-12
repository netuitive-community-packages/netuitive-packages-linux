# netuitive.packages.linux 2.7.0

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

## Release History

### Version 2.7.1

* Added computed metric for swap utilization

### Version 2.7.0

* Updated gridstack dashboard layouts

### Version 2.6.1

* Bug fix: ensure element detail page always displays the correct disk utilization metric.

### Version 2.6.0

* Added support for the new heartbeat collector.

### Version 2.5.5

* Narrow the scoping of the package.

### Version 2.5.4

* Additional change to package compatibilities.

### Version 2.5.3

* Updated package compatibilities.

### Version 2.5.2

* Updated configurations for narrower, more accurate, scope.

### Version 2.5.1

* Fixed bug with the new disk utilization computed metric.

### Version 2.5.0

* Added new computed metrics for overall disk utilization and overall disk space utilization, rather than having one of each for every disk.

### Version 2.4.4

* Adjusted the correlation flags for a couple of the computed CPU metrics.

### Version 2.4.3

* Fixed a typo on the Element Detail Page.

### Version 2.4.2

* Fixed bug with the Events widget on the Element Detail Page.

### Version 2.4.1

* Bug fix: tuned policies "Linux - Elevated User CPU" and "Linux - Elevated System CPU" to check normalized metrics.
* Bug fix: tuned number of correlated metrics to better work with large numbers of disk and network metrics.
* Bug fix: corrected the disk widgets on the Linux Summary dashboard.

### Version 2.4.0

* Bug fix: policy "Linux - Heavy Disk Load" was checking an extra condition.
* Bug fix: typo in the Linux disk and memory threshold policy descriptions.
* Introduced new computed metrics for normalized load.
* Adjusted the "Linux - Heavy CPU Load" policy to check the new normalized load metrics.

### Version 2.3.1

* Bug fix: changed the formula for the CPU utilization computed metric to ensure it wouldn't match against JVM CPU metrics.
* Changed the thresholds on the Disk and Memory Utilization Threshold Exceeded policies to 95% rather than 90% (quieter and consistent with the CPU policy).
* Renamed "Linux - Memory Utilization Exceeded" policy to "Linux - Memory Utilization Threshold Exceeded", for consistency.

### Version 2.3.0

* Updated configurations so that EC2 elements which are also receiving Linux metrics from the Netuitive agent will be able to handle those metrics correctly.
* Removed two obsolete computed metrics.

### Version 2.2.0

* Added new policy: "Linux - Heavy CPU Load"
* Added new policy: "Linux - Heavy Disk Load"
* Added new policy: "Linux - Heavy Disk Load with Slow Performance"
* Added new policy: "Linux - Memory Utilization Exceeded"
* Fixed a bug in policy "Linux - Disk Utilization Threshold Exceeded" where the wrong metric was being evaluated.
* Added new computed metrics to summarize activity across all disks.
* Updated the "Linux Summary" dashboard to display graphs of the highest disk activity.

### Version 2.1.0

* Added Linux-specific element detail page.
* Updated memory percent and network error percent metrics to show as percentages.

### Version 2.0.1

* Fixed bug where some widgets on the summary dashboard were referencing old metric names.

### Version 2.0.0

* Added units to all metrics.
* Added new policy: "Linux - CPU Threshold Exceeded"
* Added new policy: "Linux - Disk Utilization Threshold Exceeded"
* Updated computed metric names for new naming convention

### Version 1.1.0

* Added summary dashboard.

### Version 1.0.0

* Initial production release of the package for monitoring Linux OS resources.
