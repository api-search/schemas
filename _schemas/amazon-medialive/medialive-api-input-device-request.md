---
description: Settings for an input device.
layout: schema
name: InputDeviceRequest
properties_list:
- description: ''
  name: Id
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-device-request-schema.json
slug: medialive-api-input-device-request
source_filename: medialive-api-input-device-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-device-request-schema.json\",\n  \"title\": \"InputDeviceRequest\",\n  \"description\": \"Settings for an input device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The unique ID for the device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-device-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputDeviceRequest
---
