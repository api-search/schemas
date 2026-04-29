---
description: <p/>
layout: schema
name: EnableSnapshotCopyMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: DestinationRegion
  type: object
- description: ''
  name: RetentionPeriod
  type: object
- description: ''
  name: SnapshotCopyGrantName
  type: object
- description: ''
  name: ManualSnapshotRetentionPeriod
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-enable-snapshot-copy-message-schema.json
slug: redshift-enable-snapshot-copy-message
source_filename: redshift-enable-snapshot-copy-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"DestinationRegion\": {},\n    \"RetentionPeriod\": {},\n    \"SnapshotCopyGrantName\": {},\n    \"ManualSnapshotRetentionPeriod\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\",\n    \"DestinationRegion\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-enable-snapshot-copy-message-schema.json\",\n  \"title\": \"EnableSnapshotCopyMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-enable-snapshot-copy-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: EnableSnapshotCopyMessage
---
