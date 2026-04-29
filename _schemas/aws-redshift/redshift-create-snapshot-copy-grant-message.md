---
description: The result of the <code>CreateSnapshotCopyGrant</code> action.
layout: schema
name: CreateSnapshotCopyGrantMessage
properties_list:
- description: ''
  name: SnapshotCopyGrantName
  type: object
- description: ''
  name: KmsKeyId
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-snapshot-copy-grant-message-schema.json
slug: redshift-create-snapshot-copy-grant-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotCopyGrantName\": {},\n    \"KmsKeyId\": {},\n    \"Tags\": {}\n  },\n  \"required\": [\n    \"SnapshotCopyGrantName\"\n  ],\n  \"description\": \"The result of the <code>CreateSnapshotCopyGrant</code> action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-snapshot-copy-grant-message-schema.json\",\n  \"title\": \"CreateSnapshotCopyGrantMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-snapshot-copy-grant-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateSnapshotCopyGrantMessage
---
