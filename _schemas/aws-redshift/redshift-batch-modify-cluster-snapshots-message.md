---
description: BatchModifyClusterSnapshotsMessage schema from Amazon Redshift
layout: schema
name: BatchModifyClusterSnapshotsMessage
properties_list:
- description: ''
  name: SnapshotIdentifierList
  type: object
- description: ''
  name: ManualSnapshotRetentionPeriod
  type: object
- description: ''
  name: Force
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-batch-modify-cluster-snapshots-message-schema.json
slug: redshift-batch-modify-cluster-snapshots-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotIdentifierList\": {},\n    \"ManualSnapshotRetentionPeriod\": {},\n    \"Force\": {}\n  },\n  \"required\": [\n    \"SnapshotIdentifierList\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-batch-modify-cluster-snapshots-message-schema.json\",\n  \"title\": \"BatchModifyClusterSnapshotsMessage\",\n  \"description\": \"BatchModifyClusterSnapshotsMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-batch-modify-cluster-snapshots-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: BatchModifyClusterSnapshotsMessage
---
