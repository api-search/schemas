---
description: Contains information about a container in which Lambda functions run on Greengrass core devices.
layout: schema
name: LambdaContainerParams
properties_list:
- description: ''
  name: memorySizeInKB
  type: object
- description: ''
  name: mountROSysfs
  type: object
- description: ''
  name: volumes
  type: object
- description: ''
  name: devices
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-lambda-container-params-schema.json
slug: iot-greengrass-lambda-container-params
source_filename: iot-greengrass-lambda-container-params-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-container-params-schema.json\",\n  \"title\": \"LambdaContainerParams\",\n  \"description\": \"Contains information about a container in which Lambda functions run on Greengrass core devices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"memorySizeInKB\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalInteger\"\n        },\n        {\n          \"description\": \"<p>The memory size of the container, expressed in kilobytes.</p> <p>Default: <code>16384</code> (16 MB)</p>\"\n        }\n      ]\n    },\n    \"mountROSysfs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalBoolean\"\n        },\n        {\n          \"description\": \"<p>Whether or not the container can read information from the\
  \ device's <code>/sys</code> folder.</p> <p>Default: <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"volumes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaVolumeList\"\n        },\n        {\n          \"description\": \"The list of volumes that the container can access.\"\n        }\n      ]\n    },\n    \"devices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaDeviceList\"\n        },\n        {\n          \"description\": \"The list of system devices that the container can access.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-container-params-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: LambdaContainerParams
---
