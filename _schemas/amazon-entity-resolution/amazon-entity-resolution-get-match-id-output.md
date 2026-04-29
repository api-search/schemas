---
description: GetMatchIdOutput schema from AWS EntityResolution
layout: schema
name: GetMatchIdOutput
properties_list:
- description: ''
  name: matchId
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-get-match-id-output-schema.json
slug: amazon-entity-resolution-get-match-id-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-get-match-id-output-schema.json\",\n  \"title\": \"GetMatchIdOutput\",\n  \"description\": \"GetMatchIdOutput schema from AWS EntityResolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"matchId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The unique identifiers for this group of match records.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-get-match-id-output-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: GetMatchIdOutput
---
