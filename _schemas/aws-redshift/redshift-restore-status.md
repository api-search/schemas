---
description: Describes the status of a cluster restore action. Returns null if the cluster was not created by restoring a snapshot.
layout: schema
name: RestoreStatus
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: CurrentRestoreRateInMegaBytesPerSecond
  type: object
- description: ''
  name: SnapshotSizeInMegaBytes
  type: object
- description: ''
  name: ProgressInMegaBytes
  type: object
- description: ''
  name: ElapsedTimeInSeconds
  type: object
- description: ''
  name: EstimatedTimeToCompletionInSeconds
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-restore-status-schema.json
slug: redshift-restore-status
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: RestoreStatus
---
