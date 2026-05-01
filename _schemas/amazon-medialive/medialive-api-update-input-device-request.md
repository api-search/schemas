---
description: A request to update an input device.
layout: schema
name: UpdateInputDeviceRequest
properties_list:
- description: ''
  name: HdDeviceSettings
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: UhdDeviceSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-update-input-device-request-schema.json
slug: medialive-api-update-input-device-request
source_filename: medialive-api-update-input-device-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-input-device-request-schema.json\",\n  \"title\": \"UpdateInputDeviceRequest\",\n  \"description\": \"A request to update an input device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HdDeviceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceConfigurableSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hdDeviceSettings\"\n          },\n          \"description\": \"The settings that you want to apply to the HD input device.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name that you\
  \ assigned to this input device (not the unique ID).\"\n        }\n      ]\n    },\n    \"UhdDeviceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceConfigurableSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"uhdDeviceSettings\"\n          },\n          \"description\": \"The settings that you want to apply to the UHD input device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-input-device-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateInputDeviceRequest
---
