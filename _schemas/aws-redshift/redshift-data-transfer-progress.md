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
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {},\n    \"CurrentRateInMegaBytesPerSecond\": {},\n    \"TotalDataInMegaBytes\": {},\n    \"DataTransferredInMegaBytes\": {},\n    \"EstimatedTimeToCompletionInSeconds\": {},\n    \"ElapsedTimeInSeconds\": {}\n  },\n  \"description\": \"Describes the status of a cluster while it is in the process of resizing with an incremental resize.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-transfer-progress-schema.json\",\n  \"title\": \"DataTransferProgress\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-transfer-progress-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DataTransferProgress
---
