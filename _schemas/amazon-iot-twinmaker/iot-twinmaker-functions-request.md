---
description: FunctionsRequest schema
layout: schema
name: FunctionsRequest
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-functions-request-schema.json
slug: iot-twinmaker-functions-request
source_filename: iot-twinmaker-functions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-functions-request-schema.json\",\n  \"title\": \"FunctionsRequest\",\n  \"description\": \"FunctionsRequest schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"requiredProperties\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RequiredProperties\"\n          },\n          {\n            \"description\": \"The required properties of the function.\"\n          }\n        ]\n      },\n      \"scope\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Scope\"\n          },\n          {\n            \"description\": \"The scope of the function.\"\n          }\n        ]\n      },\n      \"implementedBy\": {\n        \"allOf\": [\n          {\n   \
  \         \"$ref\": \"#/components/schemas/DataConnector\"\n          },\n          {\n            \"description\": \"The data connector.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The function request body.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-functions-request-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: FunctionsRequest
---
