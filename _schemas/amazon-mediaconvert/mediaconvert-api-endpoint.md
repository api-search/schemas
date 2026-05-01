---
description: Describes an account-specific API endpoint.
layout: schema
name: Endpoint
properties_list:
- description: ''
  name: Url
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-endpoint-schema.json
slug: mediaconvert-api-endpoint
source_filename: mediaconvert-api-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-endpoint-schema.json\",\n  \"title\": \"Endpoint\",\n  \"description\": \"Describes an account-specific API endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"url\"\n          },\n          \"description\": \"URL of endpoint\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-endpoint-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Endpoint
---
