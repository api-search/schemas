---
description: The Status type defines a logical error model that is suitable for REST APIs. It is used to communicate error details from the API.
layout: schema
name: Status
properties_list:
- description: The status code, which should be an enum value of google.rpc.Code.
  name: code
  type: integer
- description: A developer-facing error message in English.
  name: message
  type: string
- description: A list of messages that carry the error details.
  name: details
  type: array
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-status-schema.json
slug: cloud-resource-manager-status
source_filename: cloud-resource-manager-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status\",\n  \"type\": \"object\",\n  \"description\": \"The Status type defines a logical error model that is suitable for REST APIs. It is used to communicate error details from the API.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"The status code, which should be an enum value of google.rpc.Code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A developer-facing error message in English.\"\n    },\n    \"details\": {\n      \"type\": \"array\",\n      \"description\": \"A list of messages that carry the error details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-status-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: Status
---
