---
description: Placeholder documentation for ListInputDevicesResponse
layout: schema
name: ListInputDevicesResponse
properties_list:
- description: ''
  name: InputDevices
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-list-input-devices-response-schema.json
slug: medialive-api-list-input-devices-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-input-devices-response-schema.json\",\n  \"title\": \"ListInputDevicesResponse\",\n  \"description\": \"Placeholder documentation for ListInputDevicesResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputDevices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputDeviceSummary\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputDevices\"\n          },\n          \"description\": \"The list of input devices.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"A token to get additional list results.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-input-devices-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListInputDevicesResponse
---
