---
description: UpdateVTLDeviceTypeInput schema from Amazon Storage Gateway API
layout: schema
name: UpdateVTLDeviceTypeInput
properties_list:
- description: ''
  name: VTLDeviceARN
  type: object
- description: ''
  name: DeviceType
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-vtl-device-type-input-schema.json
slug: amazon-storage-gateway-update-vtl-device-type-input
source_filename: amazon-storage-gateway-update-vtl-device-type-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-vtl-device-type-input-schema.json\",\n  \"title\": \"UpdateVTLDeviceTypeInput\",\n  \"description\": \"UpdateVTLDeviceTypeInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VTLDeviceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VTLDeviceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the medium changer you want to select.\"\n        }\n      ]\n    },\n    \"DeviceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceType\"\n        },\n        {\n          \"description\": \"<p>The type of medium changer you want to select.</p> <p>Valid Values: <code>STK-L700</code> | <code>AWS-Gateway-VTL</code> |\
  \ <code>IBM-03584L32-0402</code> </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VTLDeviceARN\",\n    \"DeviceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-vtl-device-type-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateVTLDeviceTypeInput
---
