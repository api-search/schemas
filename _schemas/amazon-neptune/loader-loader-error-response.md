---
description: LoaderErrorResponse schema from Neptune
layout: schema
name: LoaderErrorResponse
properties_list:
- description: ''
  name: requestId
  type: string
- description: ''
  name: code
  type: string
- description: Detailed error message.
  name: detailedMessage
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/loader-loader-error-response-schema.json
slug: loader-loader-error-response
source_filename: loader-loader-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/loader-loader-error-response-schema.json\",\n  \"title\": \"LoaderErrorResponse\",\n  \"description\": \"LoaderErrorResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"detailedMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed error message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/loader-loader-error-response-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: LoaderErrorResponse
---
