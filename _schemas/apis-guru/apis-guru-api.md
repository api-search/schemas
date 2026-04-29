---
description: Meta information about API
layout: schema
name: API
properties_list:
- description: Timestamp when the API was first added to the directory
  name: added
  type: string
- description: Recommended version
  name: preferred
  type: string
- description: List of supported versions of the API
  name: versions
  type: object
provider_name: APIs.guru
provider_slug: apis-guru
schema_file: json-schema/apis-guru-api-schema.json
slug: apis-guru-api
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-guru/refs/heads/main/json-schema/apis-guru-api-schema.json\",\n  \"title\": \"API\",\n  \"description\": \"Meta information about API\",\n  \"additionalProperties\": false,\n  \"properties\": {\n    \"added\": {\n      \"description\": \"Timestamp when the API was first added to the directory\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"preferred\": {\n      \"description\": \"Recommended version\",\n      \"type\": \"string\"\n    },\n    \"versions\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/ApiVersion\"\n      },\n      \"description\": \"List of supported versions of the API\",\n      \"minProperties\": 1,\n      \"type\": \"object\"\n    }\n  },\n  \"required\": [\n    \"added\",\n    \"preferred\",\n    \"versions\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-guru/refs/heads/main/json-schema/apis-guru-api-schema.json
tags:
- API Catalog
- API Directory
- API Discovery
- Community
- GraphQL
- Open Source
- OpenAPI
title: API
---
