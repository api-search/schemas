---
description: ComponentTypeSummaries schema
layout: schema
name: ComponentTypeSummaries
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-component-type-summaries-schema.json
slug: iot-twinmaker-component-type-summaries
source_filename: iot-twinmaker-component-type-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-component-type-summaries-schema.json\",\n  \"title\": \"ComponentTypeSummaries\",\n  \"description\": \"ComponentTypeSummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"arn\",\n      \"componentTypeId\",\n      \"creationDateTime\",\n      \"updateDateTime\"\n    ],\n    \"properties\": {\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TwinMakerArn\"\n          },\n          {\n            \"description\": \"The ARN of the component type.\"\n          }\n        ]\n      },\n      \"componentTypeId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentTypeId\"\n          },\n          {\n            \"description\": \"The ID of the\
  \ component type.\"\n          }\n        ]\n      },\n      \"creationDateTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The date and time when the component type was created.\"\n          }\n        ]\n      },\n      \"updateDateTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The date and time when the component type was last updated.\"\n          }\n        ]\n      },\n      \"description\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Description\"\n          },\n          {\n            \"description\": \"The description of the component type.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Status\"\n          },\n          {\n\
  \            \"description\": \"The current status of the component type.\"\n          }\n        ]\n      },\n      \"componentTypeName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentTypeName\"\n          },\n          {\n            \"description\": \"The component type name.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that contains information about a component type.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-component-type-summaries-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: ComponentTypeSummaries
---
