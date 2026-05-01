---
description: The data connector.
layout: schema
name: DataConnector
properties_list:
- description: ''
  name: lambda
  type: object
- description: ''
  name: isNative
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-data-connector-schema.json
slug: iot-twinmaker-data-connector
source_filename: iot-twinmaker-data-connector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-data-connector-schema.json\",\n  \"title\": \"DataConnector\",\n  \"description\": \"The data connector.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lambda\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunction\"\n        },\n        {\n          \"description\": \"The Lambda function associated with this data connector.\"\n        }\n      ]\n    },\n    \"isNative\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that specifies whether the data connector is native to IoT TwinMaker.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-data-connector-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: DataConnector
---
