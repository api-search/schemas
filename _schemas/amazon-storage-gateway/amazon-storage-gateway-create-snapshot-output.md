---
description: 'A JSON object containing the following fields:'
layout: schema
name: CreateSnapshotOutput
properties_list:
- description: ''
  name: VolumeARN
  type: object
- description: ''
  name: SnapshotId
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-snapshot-output-schema.json
slug: amazon-storage-gateway-create-snapshot-output
source_filename: amazon-storage-gateway-create-snapshot-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-snapshot-output-schema.json\",\n  \"title\": \"CreateSnapshotOutput\",\n  \"description\": \"A JSON object containing the following fields:\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the volume of which the snapshot was taken.\"\n        }\n      ]\n    },\n    \"SnapshotId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotId\"\n        },\n        {\n          \"description\": \"The snapshot ID that is used to refer to the snapshot in future operations such as describing snapshots (Amazon Elastic Compute Cloud API <code>DescribeSnapshots</code>)\
  \ or creating a volume from a snapshot (<a>CreateStorediSCSIVolume</a>).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-snapshot-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateSnapshotOutput
---
