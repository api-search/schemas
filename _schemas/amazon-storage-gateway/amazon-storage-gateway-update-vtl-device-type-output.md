---
description: UpdateVTLDeviceTypeOutput
layout: schema
name: UpdateVTLDeviceTypeOutput
properties_list:
- description: ''
  name: VTLDeviceARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-vtl-device-type-output-schema.json
slug: amazon-storage-gateway-update-vtl-device-type-output
source_filename: amazon-storage-gateway-update-vtl-device-type-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-vtl-device-type-output-schema.json\",\n  \"title\": \"UpdateVTLDeviceTypeOutput\",\n  \"description\": \"UpdateVTLDeviceTypeOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VTLDeviceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VTLDeviceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the medium changer you have selected.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-vtl-device-type-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateVTLDeviceTypeOutput
---
