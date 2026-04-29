---
description: LoaderStartResponse schema from Neptune
layout: schema
name: LoaderStartResponse
properties_list:
- description: The HTTP status (e.g., '200 OK').
  name: status
  type: string
- description: ''
  name: payload
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/loader-loader-start-response-schema.json
slug: loader-loader-start-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/loader-loader-start-response-schema.json\",\n  \"title\": \"LoaderStartResponse\",\n  \"description\": \"LoaderStartResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP status (e.g., '200 OK').\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"loadId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the initiated load job.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/loader-loader-start-response-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: LoaderStartResponse
---
