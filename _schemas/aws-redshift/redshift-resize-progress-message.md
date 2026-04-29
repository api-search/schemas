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
source_filename: redshift-resize-progress-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TargetNodeType\": {},\n    \"TargetNumberOfNodes\": {},\n    \"TargetClusterType\": {},\n    \"Status\": {},\n    \"ImportTablesCompleted\": {},\n    \"ImportTablesInProgress\": {},\n    \"ImportTablesNotStarted\": {},\n    \"AvgResizeRateInMegaBytesPerSecond\": {},\n    \"TotalResizeDataInMegaBytes\": {},\n    \"ProgressInMegaBytes\": {},\n    \"ElapsedTimeInSeconds\": {},\n    \"EstimatedTimeToCompletionInSeconds\": {},\n    \"ResizeType\": {},\n    \"Message\": {},\n    \"TargetEncryptionType\": {},\n    \"DataTransferProgressPercent\": {}\n  },\n  \"description\": \"Describes the result of a cluster resize operation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-resize-progress-message-schema.json\",\n  \"title\": \"ResizeProgressMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-resize-progress-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ResizeProgressMessage
---
