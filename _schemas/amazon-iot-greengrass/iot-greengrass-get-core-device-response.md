---
description: GetCoreDeviceResponse schema
layout: schema
name: GetCoreDeviceResponse
properties_list:
- description: ''
  name: coreDeviceThingName
  type: object
- description: ''
  name: coreVersion
  type: object
- description: ''
  name: platform
  type: object
- description: ''
  name: architecture
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: lastStatusUpdateTimestamp
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-get-core-device-response-schema.json
slug: iot-greengrass-get-core-device-response
source_filename: iot-greengrass-get-core-device-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-get-core-device-response-schema.json\",\n  \"title\": \"GetCoreDeviceResponse\",\n  \"description\": \"GetCoreDeviceResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"coreDeviceThingName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoreDeviceThingName\"\n        },\n        {\n          \"description\": \"The name of the core device. This is also the name of the IoT thing.\"\n        }\n      ]\n    },\n    \"coreVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GGCVersion\"\n        },\n        {\n          \"description\": \"The version of the IoT Greengrass Core software that the core device runs. This version is equivalent to the version of the Greengrass nucleus component that runs on\
  \ the core device. For more information, see the <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/greengrass-nucleus-component.html\\\">Greengrass nucleus component</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoreDevicePlatformString\"\n        },\n        {\n          \"description\": \"The operating system platform that the core device runs.\"\n        }\n      ]\n    },\n    \"architecture\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoreDeviceArchitectureString\"\n        },\n        {\n          \"description\": \"The computer architecture of the core device.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoreDeviceStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the core device. The core\
  \ device status can be:</p> <ul> <li> <p> <code>HEALTHY</code> \\u2013 The IoT Greengrass Core software and all components run on the core device without issue.</p> </li> <li> <p> <code>UNHEALTHY</code> \\u2013 The IoT Greengrass Core software or a component is in a failed state on the core device.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"lastStatusUpdateTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the core device's status last updated, expressed in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of key-value pairs that contain metadata for the resource. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/tag-resources.html\\\">Tag your resources</a>\
  \ in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-get-core-device-response-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: GetCoreDeviceResponse
---
