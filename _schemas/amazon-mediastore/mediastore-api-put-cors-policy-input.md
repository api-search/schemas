---
description: PutCorsPolicyInput schema from Amazon MediaStore API
layout: schema
name: PutCorsPolicyInput
properties_list:
- description: ''
  name: ContainerName
  type: object
- description: ''
  name: CorsPolicy
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-put-cors-policy-input-schema.json
slug: mediastore-api-put-cors-policy-input
source_filename: mediastore-api-put-cors-policy-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-put-cors-policy-input-schema.json\",\n  \"title\": \"PutCorsPolicyInput\",\n  \"description\": \"PutCorsPolicyInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerName\"\n        },\n        {\n          \"description\": \"The name of the container that you want to assign the CORS policy to.\"\n        }\n      ]\n    },\n    \"CorsPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CorsPolicy\"\n        },\n        {\n          \"description\": \"The CORS policy to apply to the container. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ContainerName\",\n    \"CorsPolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-put-cors-policy-input-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: PutCorsPolicyInput
---
