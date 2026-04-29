---
description: <p/>
layout: schema
name: RestoreTableFromClusterSnapshotMessage
properties_list:
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
- description: ''
  name: EnableCaseSensitiveIdentifier
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-restore-table-from-cluster-snapshot-message-schema.json
slug: redshift-restore-table-from-cluster-snapshot-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"SnapshotIdentifier\": {},\n    \"SourceDatabaseName\": {},\n    \"SourceSchemaName\": {},\n    \"SourceTableName\": {},\n    \"TargetDatabaseName\": {},\n    \"TargetSchemaName\": {},\n    \"NewTableName\": {},\n    \"EnableCaseSensitiveIdentifier\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\",\n    \"SnapshotIdentifier\",\n    \"SourceDatabaseName\",\n    \"SourceTableName\",\n    \"NewTableName\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-restore-table-from-cluster-snapshot-message-schema.json\",\n  \"title\": \"RestoreTableFromClusterSnapshotMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-restore-table-from-cluster-snapshot-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: RestoreTableFromClusterSnapshotMessage
---
