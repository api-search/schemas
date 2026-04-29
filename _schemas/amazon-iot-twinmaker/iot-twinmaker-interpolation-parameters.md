---
description: An object that specifies how to interpolate data in a list.
layout: schema
name: InterpolationParameters
properties_list:
- description: ''
  name: interpolationType
  type: object
- description: ''
  name: intervalInSeconds
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-interpolation-parameters-schema.json
slug: iot-twinmaker-interpolation-parameters
source_filename: iot-twinmaker-interpolation-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-interpolation-parameters-schema.json\",\n  \"title\": \"InterpolationParameters\",\n  \"description\": \"An object that specifies how to interpolate data in a list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"interpolationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InterpolationType\"\n        },\n        {\n          \"description\": \"The interpolation type.\"\n        }\n      ]\n    },\n    \"intervalInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntervalInSeconds\"\n        },\n        {\n          \"description\": \"The interpolation time interval in seconds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-interpolation-parameters-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: InterpolationParameters
---
