---
description: A request to transfer an input device.
layout: schema
name: TransferInputDeviceRequest
properties_list:
- description: ''
  name: TargetCustomerId
  type: object
- description: ''
  name: TargetRegion
  type: object
- description: ''
  name: TransferMessage
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-transfer-input-device-request-schema.json
slug: medialive-api-transfer-input-device-request
source_filename: medialive-api-transfer-input-device-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-transfer-input-device-request-schema.json\",\n  \"title\": \"TransferInputDeviceRequest\",\n  \"description\": \"A request to transfer an input device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TargetCustomerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"targetCustomerId\"\n          },\n          \"description\": \"The AWS account ID (12 digits) for the recipient of the device transfer.\"\n        }\n      ]\n    },\n    \"TargetRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"targetRegion\"\n          },\n          \"description\": \"The target\
  \ AWS region to transfer the device.\"\n        }\n      ]\n    },\n    \"TransferMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"transferMessage\"\n          },\n          \"description\": \"An optional message for the recipient. Maximum 280 characters.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-transfer-input-device-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: TransferInputDeviceRequest
---
