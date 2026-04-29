---
description: A point-in-time snapshot of an Amazon FSx for OpenZFS volume.
layout: schema
name: Snapshot
properties_list:
- description: Unique ID of the snapshot.
  name: SnapshotId
  type: string
- description: Name of the snapshot.
  name: Name
  type: string
- description: ID of the volume this snapshot was taken from.
  name: VolumeId
  type: string
- description: ''
  name: CreationTime
  type: string
- description: ''
  name: Lifecycle
  type: string
- description: ''
  name: ResourceARN
  type: string
- description: ''
  name: Tags
  type: array
- description: ''
  name: AdministrativeActions
  type: array
provider_name: Amazon FSx
provider_slug: amazon-fsx
schema_file: json-schema/amazon-fsx-snapshot-schema.json
slug: amazon-fsx-snapshot
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-fsx/refs/heads/main/json-schema/amazon-fsx-snapshot-schema.json\",\n  \"title\": \"Snapshot\",\n  \"description\": \"A point-in-time snapshot of an Amazon FSx for OpenZFS volume.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID of the snapshot.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the snapshot.\"\n    },\n    \"VolumeId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the volume this snapshot was taken from.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"Lifecycle\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"CREATING\",\n        \"DELETING\",\n        \"AVAILABLE\"\n      ]\n   \
  \ },\n    \"ResourceARN\": {\n      \"type\": \"string\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"AdministrativeActions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"VolumeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-fsx/refs/heads/main/json-schema/amazon-fsx-snapshot-schema.json
tags:
- AWS
- File Systems
- Lustre
- NetApp
- OpenZFS
- Storage
- Windows
title: Snapshot
---
