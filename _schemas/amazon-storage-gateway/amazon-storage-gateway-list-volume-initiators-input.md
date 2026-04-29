---
description: ListVolumeInitiatorsInput
layout: schema
name: ListVolumeInitiatorsInput
properties_list:
- description: ''
  name: VolumeARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-volume-initiators-input-schema.json
slug: amazon-storage-gateway-list-volume-initiators-input
source_filename: amazon-storage-gateway-list-volume-initiators-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-volume-initiators-input-schema.json\",\n  \"title\": \"ListVolumeInitiatorsInput\",\n  \"description\": \"ListVolumeInitiatorsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the volume. Use the <a>ListVolumes</a> operation to return a list of gateway volumes for the gateway.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VolumeARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-volume-initiators-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListVolumeInitiatorsInput
---
