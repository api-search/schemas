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
source_filename: redshift-restore-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {},\n    \"CurrentRestoreRateInMegaBytesPerSecond\": {},\n    \"SnapshotSizeInMegaBytes\": {},\n    \"ProgressInMegaBytes\": {},\n    \"ElapsedTimeInSeconds\": {},\n    \"EstimatedTimeToCompletionInSeconds\": {}\n  },\n  \"description\": \"Describes the status of a cluster restore action. Returns null if the cluster was not created by restoring a snapshot.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-restore-status-schema.json\",\n  \"title\": \"RestoreStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-restore-status-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: RestoreStatus
---
