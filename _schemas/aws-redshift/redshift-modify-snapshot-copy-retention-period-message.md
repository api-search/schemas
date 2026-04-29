---
description: <p/>
layout: schema
name: ModifySnapshotCopyRetentionPeriodMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: RetentionPeriod
  type: object
- description: ''
  name: Manual
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-snapshot-copy-retention-period-message-schema.json
slug: redshift-modify-snapshot-copy-retention-period-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"RetentionPeriod\": {},\n    \"Manual\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\",\n    \"RetentionPeriod\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-snapshot-copy-retention-period-message-schema.json\",\n  \"title\": \"ModifySnapshotCopyRetentionPeriodMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-snapshot-copy-retention-period-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifySnapshotCopyRetentionPeriodMessage
---
