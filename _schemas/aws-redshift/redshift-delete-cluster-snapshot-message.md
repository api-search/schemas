---
description: <p/>
layout: schema
name: DeleteClusterSnapshotMessage
properties_list:
- description: ''
  name: SnapshotIdentifier
  type: object
- description: ''
  name: SnapshotClusterIdentifier
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-delete-cluster-snapshot-message-schema.json
slug: redshift-delete-cluster-snapshot-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotIdentifier\": {},\n    \"SnapshotClusterIdentifier\": {}\n  },\n  \"required\": [\n    \"SnapshotIdentifier\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-delete-cluster-snapshot-message-schema.json\",\n  \"title\": \"DeleteClusterSnapshotMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-delete-cluster-snapshot-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: DeleteClusterSnapshotMessage
---
