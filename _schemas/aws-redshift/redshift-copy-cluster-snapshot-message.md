---
description: <p/>
layout: schema
name: CopyClusterSnapshotMessage
properties_list:
- description: ''
  name: SourceSnapshotIdentifier
  type: object
- description: ''
  name: SourceSnapshotClusterIdentifier
  type: object
- description: ''
  name: TargetSnapshotIdentifier
  type: object
- description: ''
  name: ManualSnapshotRetentionPeriod
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-copy-cluster-snapshot-message-schema.json
slug: redshift-copy-cluster-snapshot-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceSnapshotIdentifier\": {},\n    \"SourceSnapshotClusterIdentifier\": {},\n    \"TargetSnapshotIdentifier\": {},\n    \"ManualSnapshotRetentionPeriod\": {}\n  },\n  \"required\": [\n    \"SourceSnapshotIdentifier\",\n    \"TargetSnapshotIdentifier\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-copy-cluster-snapshot-message-schema.json\",\n  \"title\": \"CopyClusterSnapshotMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-copy-cluster-snapshot-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CopyClusterSnapshotMessage
---
