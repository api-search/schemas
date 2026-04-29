---
description: The tabular conditions.
layout: schema
name: TabularConditions
properties_list:
- description: ''
  name: orderBy
  type: object
- description: ''
  name: propertyFilters
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-tabular-conditions-schema.json
slug: iot-twinmaker-tabular-conditions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-tabular-conditions-schema.json\",\n  \"title\": \"TabularConditions\",\n  \"description\": \"The tabular conditions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderByList\"\n        },\n        {\n          \"description\": \"Filter criteria that orders the output. It can be sorted in ascending or descending order.\"\n        }\n      ]\n    },\n    \"propertyFilters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyFilters\"\n        },\n        {\n          \"description\": \"<p>You can filter the request using various logical operators and a key-value format. For example:</p> <p> <code>{\\\"key\\\": \\\"serverType\\\", \\\"value\\\": \\\"webServer\\\
  \"}</code> </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-tabular-conditions-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: TabularConditions
---
