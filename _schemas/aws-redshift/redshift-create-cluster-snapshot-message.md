---
description: <p/>
layout: schema
name: CreateClusterSnapshotMessage
properties_list:
- description: ''
  name: SnapshotIdentifier
  type: object
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: ManualSnapshotRetentionPeriod
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-cluster-snapshot-message-schema.json
slug: redshift-create-cluster-snapshot-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotIdentifier\": {},\n    \"ClusterIdentifier\": {},\n    \"ManualSnapshotRetentionPeriod\": {},\n    \"Tags\": {}\n  },\n  \"required\": [\n    \"SnapshotIdentifier\",\n    \"ClusterIdentifier\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-snapshot-message-schema.json\",\n  \"title\": \"CreateClusterSnapshotMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-cluster-snapshot-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateClusterSnapshotMessage
---
