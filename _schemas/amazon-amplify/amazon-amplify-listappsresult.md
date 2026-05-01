---
description: ''
layout: schema
name: ListAppsResult
properties_list:
- description: ''
  name: apps
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon Amplify
provider_slug: amazon-amplify
schema_file: json-schema/amazon-amplify-listappsresult-schema.json
slug: amazon-amplify-listappsresult
source_filename: amazon-amplify-listappsresult-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ListAppsResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apps\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/App\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-amplify/refs/heads/main/json-schema/amazon-amplify-listappsresult-schema.json
tags:
- Frontend
- Full Stack
- Hosting
- Mobile Development
- Web Applications
title: ListAppsResult
---
