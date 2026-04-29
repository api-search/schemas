---
description: The function response.
layout: schema
name: FunctionResponse
properties_list:
- description: ''
  name: requiredProperties
  type: object
- description: ''
  name: scope
  type: object
- description: ''
  name: implementedBy
  type: object
- description: ''
  name: isInherited
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-function-response-schema.json
slug: iot-twinmaker-function-response
source_filename: iot-twinmaker-function-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-function-response-schema.json\",\n  \"title\": \"FunctionResponse\",\n  \"description\": \"The function response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requiredProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequiredProperties\"\n        },\n        {\n          \"description\": \"The required properties of the function.\"\n        }\n      ]\n    },\n    \"scope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scope\"\n        },\n        {\n          \"description\": \"The scope of the function.\"\n        }\n      ]\n    },\n    \"implementedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataConnector\"\n        },\n        {\n          \"description\": \"\
  The data connector.\"\n        }\n      ]\n    },\n    \"isInherited\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether this function is inherited.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-function-response-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: FunctionResponse
---
