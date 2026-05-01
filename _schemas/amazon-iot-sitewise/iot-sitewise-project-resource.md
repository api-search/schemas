---
description: Identifies a specific IoT SiteWise Monitor project.
layout: schema
name: ProjectResource
properties_list:
- description: ''
  name: id
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-project-resource-schema.json
slug: iot-sitewise-project-resource
source_filename: iot-sitewise-project-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-project-resource-schema.json\",\n  \"title\": \"ProjectResource\",\n  \"description\": \"Identifies a specific IoT SiteWise Monitor project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the project.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-project-resource-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: ProjectResource
---
