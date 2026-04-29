---
description: <p/>
layout: schema
name: DeleteClusterMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: SkipFinalClusterSnapshot
  type: object
- description: ''
  name: FinalClusterSnapshotIdentifier
  type: object
- description: ''
  name: FinalClusterSnapshotRetentionPeriod
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-delete-cluster-message-schema.json
slug: redshift-delete-cluster-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"SkipFinalClusterSnapshot\": {},\n    \"FinalClusterSnapshotIdentifier\": {},\n    \"FinalClusterSnapshotRetentionPeriod\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-delete-cluster-message-schema.json\",\n  \"title\": \"DeleteClusterMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-delete-cluster-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DeleteClusterMessage
---
