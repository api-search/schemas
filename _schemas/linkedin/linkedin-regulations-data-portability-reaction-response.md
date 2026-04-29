---
description: ReactionResponse from LinkedIn API
layout: schema
name: ReactionResponse
properties_list:
- description: ''
  name: elements
  type: array
- description: ''
  name: paging
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-regulations-data-portability-reaction-response-schema.json
slug: linkedin-regulations-data-portability-reaction-response
source_filename: linkedin-regulations-data-portability-reaction-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-reaction-response-schema.json\",\n  \"title\": \"ReactionResponse\",\n  \"description\": \"ReactionResponse from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Reaction\"\n      }\n    },\n    \"paging\": {\n      \"$ref\": \"#/components/schemas/Paging\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-reaction-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ReactionResponse
---
