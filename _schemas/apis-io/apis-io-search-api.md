---
description: The description of the API
layout: schema
name: API
properties_list:
- description: name
  name: name
  type: string
- description: description of the API
  name: description
  type: string
- description: URL of an image representing the API
  name: image
  type: string
- description: baseURL
  name: baseURL
  type: string
- description: humanURL
  name: humanURL
  type: string
- description: tags to describe the API
  name: tags
  type: array
- description: URLs
  name: properties
  type: array
- description: Contact to reach if questions about API
  name: contact
  type: array
- description: ''
  name: meta
  type: array
provider_name: APIs.io
provider_slug: apis-io
schema_file: json-schema/apis-io-search-api-schema.json
slug: apis-io-search-api
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-api-schema.json\",\n  \"title\": \"API\",\n  \"description\": \"The description of the API\",\n  \"required\": [\n    \"name\",\n    \"description\",\n    \"image\",\n    \"baseURL\",\n    \"humanURL\",\n    \"properties\",\n    \"contact\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"name\",\n      \"minLength\": 5\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"description of the API\",\n      \"minLength\": 5\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"URL of an image representing the API\"\n    },\n    \"baseURL\": {\n      \"type\": \"string\",\n      \"pattern\": \"^(http)|(https)://(.*)$\",\n      \"description\": \"baseURL\"\n    },\n    \"humanURL\": {\n    \
  \  \"type\": \"string\",\n      \"pattern\": \"^(http)|(https)://(.*)$\",\n      \"description\": \"humanURL\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"minLength\": 1\n      },\n      \"description\": \"tags to describe the API\"\n    },\n    \"properties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Property\"\n      },\n      \"description\": \"URLs\"\n    },\n    \"contact\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Contact\"\n      },\n      \"description\": \"Contact to reach if questions about API\"\n    },\n    \"meta\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/metaInformation\"\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-api-schema.json
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
title: API
---
