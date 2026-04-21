---
description: Describes the result of a cluster resize operation.
layout: schema
name: ResizeProgressMessage
properties_list:
- description: ''
  name: TargetNodeType
  type: object
- description: ''
  name: TargetNumberOfNodes
  type: object
- description: ''
  name: TargetClusterType
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: ImportTablesCompleted
  type: object
- description: ''
  name: ImportTablesInProgress
  type: object
- description: ''
  name: ImportTablesNotStarted
  type: object
- description: ''
  name: AvgResizeRateInMegaBytesPerSecond
  type: object
- description: ''
  name: TotalResizeDataInMegaBytes
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
- description: ''
  name: ResizeType
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: TargetEncryptionType
  type: object
- description: ''
  name: DataTransferProgressPercent
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-resize-progress-message-schema.json
slug: redshift-resize-progress-message
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ResizeProgressMessage
---
