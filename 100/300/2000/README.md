# 2000 Data Backup and Resiliency

## Data Replication and Backup

Backup is different from Data Replication. 

***Data Replication***:
- allow systems to fail over quickly to a replica by copying data in near real-time, either synchronously or asynchronously.
- assures that a replica of the data is readily available and can help reduce the time it takes to recover from an outage.
- should not be considered as a substitute for backups.

***Data Backup***
- you get quick access to files.
- you can be safe in case of power failures.
- you can be safe against hardware failures.
- you can safe money as don't need physical hardware to back up data and applications.

## Resiliency

Design for resiliency in a cloud environment focuses on failure recovery, rather than on avoiding failures.

The goal is to return applications to a fully functioning state following a failure by responding to failures, such that it avoids downtime or data loss.

In case a failure occurs, then your team would be aware of whom to contact and start the recovery process.

This makes it very simple for you to bring your application to live again.

## Resiliency: Recovery Time Objective (RTO)

***Recovery Time Objective (RTO)*** is the maximum acceptable time an application can be unavailable after a failure or incident.

If the RTO is 70 minutes, the application must be restored to a running state within 70 minutes from the start of the disaster.

You should consider a secondary deployment of applications running in standby mode if the RTO is low.

## Resiliency: Recovery Point Objective (RPO)

***Recovery Point Objective (RPO)*** is the maximum duration of data loss that is acceptable during a disaster.

For example:

If an inventory data is in a single database, with no replication to other databases, and performs backups every hour, then you could loose data worth an hour.
