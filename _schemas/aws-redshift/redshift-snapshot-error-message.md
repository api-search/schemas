---
description: Describes the errors returned by a snapshot.
layout: schema
name: SnapshotErrorMessage
properties_list:
- description: ''
  name: SnapshotIdentifier
  type: object
- description: ''
  name: SnapshotClusterIdentifier
  type: object
- description: ''
  name: FailureCode
  type: object
- description: ''
  name: FailureReason
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-snapshot-error-message-schema.json
slug: redshift-snapshot-error-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotIdentifier\": {},\n    \"SnapshotClusterIdentifier\": {},\n    \"FailureCode\": {},\n    \"FailureReason\": {}\n  },\n  \"description\": \"Describes the errors returned by a snapshot.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-snapshot-error-message-schema.json\",\n  \"title\": \"SnapshotErrorMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-snapshot-error-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: SnapshotErrorMessage
---
