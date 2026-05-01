---
description: A JSON object containing the Amazon Resource Name (ARN) of the gateway.
layout: schema
name: ListLocalDisksInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-local-disks-input-schema.json
slug: amazon-storage-gateway-list-local-disks-input
source_filename: amazon-storage-gateway-list-local-disks-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-local-disks-input-schema.json\",\n  \"title\": \"ListLocalDisksInput\",\n  \"description\": \"A JSON object containing the Amazon Resource Name (ARN) of the gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    }\n  },\n  \"required\": [\n    \"GatewayARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-local-disks-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListLocalDisksInput
---
