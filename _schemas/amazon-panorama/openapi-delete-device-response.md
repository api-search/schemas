---
description: DeleteDeviceResponse schema from Amazon Panorama
layout: schema
name: DeleteDeviceResponse
properties_list:
- description: ''
  name: DeviceId
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-delete-device-response-schema.json
slug: openapi-delete-device-response
source_filename: openapi-delete-device-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-delete-device-response-schema.json\",\n  \"title\": \"DeleteDeviceResponse\",\n  \"description\": \"DeleteDeviceResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeviceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceId\"\n        },\n        {\n          \"description\": \"The device's ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-delete-device-response-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DeleteDeviceResponse
---
