---
description: Describes the status of a cluster while it is in the process of resizing with an incremental resize.
layout: schema
name: DataTransferProgress
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: CurrentRateInMegaBytesPerSecond
  type: object
- description: ''
  name: TotalDataInMegaBytes
  type: object
- description: ''
  name: DataTransferredInMegaBytes
  type: object
- description: ''
  name: EstimatedTimeToCompletionInSeconds
  type: object
- description: ''
  name: ElapsedTimeInSeconds
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-transfer-progress-schema.json
slug: redshift-data-transfer-progress
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DataTransferProgress
---
