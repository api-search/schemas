---
description: Information about a filter.
layout: schema
name: Filter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-filter-schema.json
slug: amazon-robomaker-openapi-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"Information about a filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the filter.\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterValues\"\n        },\n        {\n          \"description\": \"A list of values.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-filter-schema.json
tags:
- AWS
- Robotics
- Simulation
title: Filter
---
