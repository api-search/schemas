---
description: Details about the input device that is being transferred.
layout: schema
name: TransferringInputDeviceSummary
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: TargetCustomerId
  type: object
- description: ''
  name: TransferType
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-transferring-input-device-summary-schema.json
slug: medialive-api-transferring-input-device-summary
source_filename: medialive-api-transferring-input-device-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-transferring-input-device-summary-schema.json\",\n  \"title\": \"TransferringInputDeviceSummary\",\n  \"description\": \"Details about the input device that is being transferred.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The unique ID of the input device.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"message\"\n          },\n          \"description\": \"The optional message that the sender has attached to the\
  \ transfer.\"\n        }\n      ]\n    },\n    \"TargetCustomerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"targetCustomerId\"\n          },\n          \"description\": \"The AWS account ID for the recipient of the input device transfer.\"\n        }\n      ]\n    },\n    \"TransferType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceTransferType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"transferType\"\n          },\n          \"description\": \"The type (direction) of the input device transfer.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-transferring-input-device-summary-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: TransferringInputDeviceSummary
---
