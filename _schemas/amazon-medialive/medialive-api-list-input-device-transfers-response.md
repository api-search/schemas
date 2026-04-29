---
description: Placeholder documentation for ListInputDeviceTransfersResponse
layout: schema
name: ListInputDeviceTransfersResponse
properties_list:
- description: ''
  name: InputDeviceTransfers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-list-input-device-transfers-response-schema.json
slug: medialive-api-list-input-device-transfers-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-input-device-transfers-response-schema.json\",\n  \"title\": \"ListInputDeviceTransfersResponse\",\n  \"description\": \"Placeholder documentation for ListInputDeviceTransfersResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputDeviceTransfers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfTransferringInputDeviceSummary\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputDeviceTransfers\"\n          },\n          \"description\": \"The list of devices that you are transferring or are being transferred to you.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n          \
  \  \"name\": \"nextToken\"\n          },\n          \"description\": \"A token to get additional list results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-input-device-transfers-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListInputDeviceTransfersResponse
---
