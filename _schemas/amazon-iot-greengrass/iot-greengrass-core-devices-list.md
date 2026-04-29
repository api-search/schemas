---
description: CoreDevicesList schema
layout: schema
name: CoreDevicesList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-core-devices-list-schema.json
slug: iot-greengrass-core-devices-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-core-devices-list-schema.json\",\n  \"title\": \"CoreDevicesList\",\n  \"description\": \"CoreDevicesList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"coreDeviceThingName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CoreDeviceThingName\"\n          },\n          {\n            \"description\": \"The name of the core device. This is also the name of the IoT thing.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CoreDeviceStatus\"\n          },\n          {\n            \"description\": \"<p>The status of the core device. Core devices can have the following statuses:</p> <ul> <li> <p> <code>HEALTHY</code>\
  \ \\u2013 The IoT Greengrass Core software and all components run on the core device without issue.</p> </li> <li> <p> <code>UNHEALTHY</code> \\u2013 The IoT Greengrass Core software or a component is in a failed state on the core device.</p> </li> </ul>\"\n          }\n        ]\n      },\n      \"lastStatusUpdateTimestamp\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The time at which the core device's status last updated, expressed in ISO 8601 format.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a Greengrass core device, which is an IoT thing that runs the IoT Greengrass Core software.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-core-devices-list-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: CoreDevicesList
---
