---
description: ModifyClusterSnapshotMessage schema from Amazon Redshift
layout: schema
name: ModifyClusterSnapshotMessage
properties_list:
- description: ''
  name: SnapshotIdentifier
  type: object
- description: ''
  name: ManualSnapshotRetentionPeriod
  type: object
- description: ''
  name: Force
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-cluster-snapshot-message-schema.json
slug: redshift-modify-cluster-snapshot-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotIdentifier\": {},\n    \"ManualSnapshotRetentionPeriod\": {},\n    \"Force\": {}\n  },\n  \"required\": [\n    \"SnapshotIdentifier\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-snapshot-message-schema.json\",\n  \"title\": \"ModifyClusterSnapshotMessage\",\n  \"description\": \"ModifyClusterSnapshotMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-cluster-snapshot-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyClusterSnapshotMessage
---
