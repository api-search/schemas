---
description: Contains the output from the <a>DescribeClusterSnapshots</a> action.
layout: schema
name: SnapshotMessage
properties_list:
- description: ''
  name: Marker
  type: object
- description: ''
  name: Snapshots
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-snapshot-message-schema.json
slug: redshift-snapshot-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Marker\": {},\n    \"Snapshots\": {}\n  },\n  \"description\": \"Contains the output from the <a>DescribeClusterSnapshots</a> action. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-snapshot-message-schema.json\",\n  \"title\": \"SnapshotMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-snapshot-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: SnapshotMessage
---
