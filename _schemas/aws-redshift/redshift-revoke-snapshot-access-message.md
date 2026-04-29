---
description: <p/>
layout: schema
name: RevokeSnapshotAccessMessage
properties_list:
- description: ''
  name: SnapshotIdentifier
  type: object
- description: ''
  name: SnapshotArn
  type: object
- description: ''
  name: SnapshotClusterIdentifier
  type: object
- description: ''
  name: AccountWithRestoreAccess
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-revoke-snapshot-access-message-schema.json
slug: redshift-revoke-snapshot-access-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotIdentifier\": {},\n    \"SnapshotArn\": {},\n    \"SnapshotClusterIdentifier\": {},\n    \"AccountWithRestoreAccess\": {}\n  },\n  \"required\": [\n    \"AccountWithRestoreAccess\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-revoke-snapshot-access-message-schema.json\",\n  \"title\": \"RevokeSnapshotAccessMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-revoke-snapshot-access-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: RevokeSnapshotAccessMessage
---
