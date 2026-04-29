---
description: AttachVolumeInput
layout: schema
name: DetachVolumeInput
properties_list:
- description: ''
  name: VolumeARN
  type: object
- description: ''
  name: ForceDetach
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-detach-volume-input-schema.json
slug: amazon-storage-gateway-detach-volume-input
source_filename: amazon-storage-gateway-detach-volume-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-detach-volume-input-schema.json\",\n  \"title\": \"DetachVolumeInput\",\n  \"description\": \"AttachVolumeInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the volume to detach from the gateway.\"\n        }\n      ]\n    },\n    \"ForceDetach\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Set to <code>true</code> to forcibly remove the iSCSI connection of the target volume and detach the volume. The default is <code>false</code>. If this value is set to <code>false</code>, you\
  \ must manually disconnect the iSCSI connection from the target volume.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VolumeARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-detach-volume-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DetachVolumeInput
---
