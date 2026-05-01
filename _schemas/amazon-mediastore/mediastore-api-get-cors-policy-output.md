---
description: GetCorsPolicyOutput schema from Amazon MediaStore API
layout: schema
name: GetCorsPolicyOutput
properties_list:
- description: ''
  name: CorsPolicy
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-get-cors-policy-output-schema.json
slug: mediastore-api-get-cors-policy-output
source_filename: mediastore-api-get-cors-policy-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-get-cors-policy-output-schema.json\",\n  \"title\": \"GetCorsPolicyOutput\",\n  \"description\": \"GetCorsPolicyOutput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CorsPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CorsPolicy\"\n        },\n        {\n          \"description\": \"The CORS policy assigned to the container.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CorsPolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-get-cors-policy-output-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: GetCorsPolicyOutput
---
