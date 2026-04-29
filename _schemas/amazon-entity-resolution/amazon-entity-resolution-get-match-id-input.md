---
description: GetMatchIdInput schema from AWS EntityResolution
layout: schema
name: GetMatchIdInput
properties_list:
- description: ''
  name: record
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-get-match-id-input-schema.json
slug: amazon-entity-resolution-get-match-id-input
source_filename: amazon-entity-resolution-get-match-id-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-get-match-id-input-schema.json\",\n  \"title\": \"GetMatchIdInput\",\n  \"description\": \"GetMatchIdInput schema from AWS EntityResolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"record\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordAttributeMap\"\n        },\n        {\n          \"description\": \"The record to fetch the Match ID for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"record\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-get-match-id-input-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: GetMatchIdInput
---
