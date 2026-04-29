---
description: ListClientDevicesAssociatedWithCoreDeviceResponse schema
layout: schema
name: ListClientDevicesAssociatedWithCoreDeviceResponse
properties_list:
- description: ''
  name: associatedClientDevices
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-list-client-devices-associated-with-core-device-response-schema.json
slug: iot-greengrass-list-client-devices-associated-with-core-device-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-client-devices-associated-with-core-device-response-schema.json\",\n  \"title\": \"ListClientDevicesAssociatedWithCoreDeviceResponse\",\n  \"description\": \"ListClientDevicesAssociatedWithCoreDeviceResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"associatedClientDevices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssociatedClientDeviceList\"\n        },\n        {\n          \"description\": \"A list that describes the client devices that are associated with the core device.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextTokenString\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if\
  \ there are no additional results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-list-client-devices-associated-with-core-device-response-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ListClientDevicesAssociatedWithCoreDeviceResponse
---
