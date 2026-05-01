---
description: TagResourceRequest schema from openapi
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-tag-resource-request-schema.json
slug: amazon-robomaker-openapi-tag-resource-request
source_filename: amazon-robomaker-openapi-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-tag-resource-request-schema.json
tags:
- Robotics
- Simulation
title: TagResourceRequest
---
