# powerMonitor

A simple program designed to pull cpu usage data from Windows 10 PrefMon, using the pdh.h header file, and toggle the computer between high performance and powersaving mode when certain thresholds are met. In this instance I am taking the last five minutes worth of data and comparing it to the data gathered within the last sixty minutes. If the average of the last five units is higher than the average over the last hour and both are above 33% CPU usage, then the high performance mode will kick in. Like-wise if the average of the last five minutes is less than the average of the last sixty minutes and below the 25% mark, then the computer will enter power saving mode. This program is designed to be run on a Windows 10 platform. In this instance I am using 25% as the lower bound and 33% as the upper bound.
