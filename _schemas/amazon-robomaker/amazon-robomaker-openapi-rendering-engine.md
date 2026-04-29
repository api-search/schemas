---
description: Information about a rendering engine.
layout: schema
name: RenderingEngine
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-rendering-engine-schema.json
slug: amazon-robomaker-openapi-rendering-engine
source_filename: amazon-robomaker-openapi-rendering-engine-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-rendering-engine-schema.json\",\n  \"title\": \"RenderingEngine\",\n  \"description\": \"Information about a rendering engine.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RenderingEngineType\"\n        },\n        {\n          \"description\": \"The name of the rendering engine.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RenderingEngineVersionType\"\n        },\n        {\n          \"description\": \"The version of the rendering engine.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-rendering-engine-schema.json
tags:
- AWS
- Robotics
- Simulation
title: RenderingEngine
---
