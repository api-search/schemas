---
description: ListCoreDevicesResponse schema
layout: schema
name: ListCoreDevicesResponse
properties_list:
- description: ''
  name: coreDevices
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-list-core-devices-response-schema.json
slug: iot-greengrass-list-core-devices-response
source_filename: iot-greengrass-list-core-devices-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-core-devices-response-schema.json\",\n  \"title\": \"ListCoreDevicesResponse\",\n  \"description\": \"ListCoreDevicesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"coreDevices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoreDevicesList\"\n        },\n        {\n          \"description\": \"A list that summarizes each core device.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextTokenString\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-core-devices-response-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ListCoreDevicesResponse
---
