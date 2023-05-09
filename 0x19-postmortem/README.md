0x19-postmortem

Postmortem Report: Network Outage on May 10, 2023

Issue Summary:

On May 10, 2023, from 2:00 PM to 5:00 PM EDT, users experienced a complete outage of our cloud-based storage service, resulting in the inability to access stored data. Approximately 75% of users were affected by this outage.

Timeline:

2:00 PM: The issue was detected when the monitoring system reported a sudden spike in error rates.

2:01 PM: The incident was escalated to the on-call engineer.

2:05 PM: The engineer investigated the system logs and network traffic to identify the root cause of the issue.

2:20 PM: Assumptions were made that the outage was caused by a network configuration error and began investigating the network infrastructure.

2:45 PM: Several network switches were rebooted in an attempt to fix the issue, but the outage persisted.

3:00 PM: A team of network specialists was called in to further investigate the issue.

3:30 PM: After a thorough investigation, it was discovered that the root cause of the outage was due to a failure in the storage array.

3:45 PM: The incident was escalated to senior management.

4:00 PM: The decision was made to restore data from the most recent backup, which was performed approximately two hours prior to the outage.

5:00 PM: The service was fully restored, and users were able to access their data.

Root Cause and Resolution:

The root cause of the outage was a hardware failure in the storage array. Specifically, one of the hard drives in the array failed, which caused the system to enter into a degraded state. This degraded state resulted in the system being unable to handle incoming requests, causing the outage. To resolve the issue, the failed drive was replaced, and the system was fully restored from the most recent backup.
Corrective and Preventative Measures:

To prevent similar outages in the future, the following corrective and preventative measures have been identified:

Increase the frequency of backups to reduce the amount of data loss in the event of an outage.

Implement redundant storage arrays to ensure that hardware failures do not result in service outages.

Improve monitoring and alerting systems to quickly detect and respond to any hardware failures in the system.

Conduct a thorough review of the network infrastructure to identify any potential misconfigurations or vulnerabilities.

Tasks to Address the Issue:

Implement a redundant storage array with automatic failover.

Increase the frequency of backups to every hour.

Review and update the monitoring and alerting systems to detect and respond to hardware failures more quickly.

Conduct a full audit of the network infrastructure to identify any potential misconfigurations or vulnerabilities.

In conclusion, the outage was caused by a hardware failure in the storage array, which was resolved by replacing the failed drive and restoring the system from a recent backup. Moving forward, we will implement several corrective and preventative measures to ensure that similar outages do not occur in the future.



Eseigbe Emmanuel

