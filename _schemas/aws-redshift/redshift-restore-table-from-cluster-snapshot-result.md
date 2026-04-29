---
description: RestoreTableFromClusterSnapshotResult schema from Amazon Redshift
layout: schema
name: RestoreTableFromClusterSnapshotResult
properties_list:
- description: Describes the status of a <a>RestoreTableFromClusterSnapshot</a> operation.
  name: TableRestoreStatus
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-restore-table-from-cluster-snapshot-result-schema.json
slug: redshift-restore-table-from-cluster-snapshot-result
source_filename: redshift-restore-table-from-cluster-snapshot-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableRestoreStatus\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"TableRestoreRequestId\": {},\n        \"Status\": {},\n        \"Message\": {},\n        \"RequestTime\": {},\n        \"ProgressInMegaBytes\": {},\n        \"TotalDataInMegaBytes\": {},\n        \"ClusterIdentifier\": {},\n        \"SnapshotIdentifier\": {},\n        \"SourceDatabaseName\": {},\n        \"SourceSchemaName\": {},\n        \"SourceTableName\": {},\n        \"TargetDatabaseName\": {},\n        \"TargetSchemaName\": {},\n        \"NewTableName\": {}\n      },\n      \"description\": \"Describes the status of a <a>RestoreTableFromClusterSnapshot</a> operation.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-restore-table-from-cluster-snapshot-result-schema.json\",\n  \"title\"\
  : \"RestoreTableFromClusterSnapshotResult\",\n  \"description\": \"RestoreTableFromClusterSnapshotResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-restore-table-from-cluster-snapshot-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: RestoreTableFromClusterSnapshotResult
---
