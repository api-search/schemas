---
description: <p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>CreateSnapshotInput$SnapshotDescription</a> </p> </li> <li> <p> <a>CreateSnapshotInput$VolumeARN</a> </p> </li> </ul>
layout: schema
name: CreateSnapshotInput
properties_list:
- description: ''
  name: VolumeARN
  type: object
- description: ''
  name: SnapshotDescription
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-snapshot-input-schema.json
slug: amazon-storage-gateway-create-snapshot-input
source_filename: amazon-storage-gateway-create-snapshot-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-snapshot-input-schema.json\",\n  \"title\": \"CreateSnapshotInput\",\n  \"description\": \"<p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>CreateSnapshotInput$SnapshotDescription</a> </p> </li> <li> <p> <a>CreateSnapshotInput$VolumeARN</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the volume. Use the <a>ListVolumes</a> operation to return a list of gateway volumes.\"\n        }\n      ]\n    },\n    \"SnapshotDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotDescription\"\
  \n        },\n        {\n          \"description\": \"Textual description of the snapshot that appears in the Amazon EC2 console, Elastic Block Store snapshots panel in the <b>Description</b> field, and in the Storage Gateway snapshot <b>Details</b> pane, <b>Description</b> field.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>A list of up to 50 tags that can be assigned to a snapshot. Each tag is a key-value pair.</p> <note> <p>Valid characters for key and value are letters, spaces, and numbers representable in UTF-8 format, and the following special characters: + - = . _ : / @. The maximum length of a tag's key is 128 characters, and the maximum length for a tag's value is 256.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VolumeARN\",\n    \"SnapshotDescription\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-snapshot-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateSnapshotInput
---
