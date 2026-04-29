---
description: TagResourceInput schema from AWS EntityResolution
layout: schema
name: TagResourceInput
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-tag-resource-input-schema.json
slug: amazon-entity-resolution-tag-resource-input
source_filename: amazon-entity-resolution-tag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-tag-resource-input-schema.json\",\n  \"title\": \"TagResourceInput\",\n  \"description\": \"TagResourceInput schema from AWS EntityResolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags used to organize, track, or control access for this resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-tag-resource-input-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: TagResourceInput
---
