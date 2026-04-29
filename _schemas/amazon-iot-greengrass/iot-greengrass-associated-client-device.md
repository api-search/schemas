---
description: Contains information about a client device that is associated to a core device for cloud discovery.
layout: schema
name: AssociatedClientDevice
properties_list:
- description: ''
  name: thingName
  type: object
- description: ''
  name: associationTimestamp
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-associated-client-device-schema.json
slug: iot-greengrass-associated-client-device
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-associated-client-device-schema.json\",\n  \"title\": \"AssociatedClientDevice\",\n  \"description\": \"Contains information about a client device that is associated to a core device for cloud discovery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IoTThingName\"\n        },\n        {\n          \"description\": \"The name of the IoT thing that represents the associated client device.\"\n        }\n      ]\n    },\n    \"associationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the client device was associated, expressed in ISO 8601 format.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-associated-client-device-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: AssociatedClientDevice
---
