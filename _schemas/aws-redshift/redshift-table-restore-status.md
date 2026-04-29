---
description: Describes the status of a <a>RestoreTableFromClusterSnapshot</a> operation.
layout: schema
name: TableRestoreStatus
properties_list:
- description: ''
  name: TableRestoreRequestId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: RequestTime
  type: object
- description: ''
  name: ProgressInMegaBytes
  type: object
- description: ''
  name: TotalDataInMegaBytes
  type: object
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: SnapshotIdentifier
  type: object
- description: ''
  name: SourceDatabaseName
  type: object
- description: ''
  name: SourceSchemaName
  type: object
- description: ''
  name: SourceTableName
  type: object
- description: ''
  name: TargetDatabaseName
  type: object
- description: ''
  name: TargetSchemaName
  type: object
- description: ''
  name: NewTableName
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-table-restore-status-schema.json
slug: redshift-table-restore-status
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableRestoreRequestId\": {},\n    \"Status\": {},\n    \"Message\": {},\n    \"RequestTime\": {},\n    \"ProgressInMegaBytes\": {},\n    \"TotalDataInMegaBytes\": {},\n    \"ClusterIdentifier\": {},\n    \"SnapshotIdentifier\": {},\n    \"SourceDatabaseName\": {},\n    \"SourceSchemaName\": {},\n    \"SourceTableName\": {},\n    \"TargetDatabaseName\": {},\n    \"TargetSchemaName\": {},\n    \"NewTableName\": {}\n  },\n  \"description\": \"Describes the status of a <a>RestoreTableFromClusterSnapshot</a> operation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-table-restore-status-schema.json\",\n  \"title\": \"TableRestoreStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-table-restore-status-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: TableRestoreStatus
---
