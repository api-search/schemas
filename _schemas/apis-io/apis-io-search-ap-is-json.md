---
description: APIsJSON schema from APIs.io Search API
layout: schema
name: APIsJSON
properties_list:
- description: The name of the service described
  name: name
  type: string
- description: Description of the service
  name: description
  type: string
- description: URL where the apis.json file will live
  name: url
  type: string
- description: Image to represent the API
  name: image
  type: string
- description: Date when the file was created
  name: created
  type: string
- description: Date when the file was modified
  name: modified
  type: string
- description: APIs.json spec version, latest is 0.18
  name: specificationVersion
  type: string
- description: All the APIs of this service
  name: apis
  type: array
- description: Maintainers of the apis.json file
  name: maintainers
  type: array
- description: Tags to describe the service
  name: tags
  type: array
- description: Links to other apis.json definitions included in this service.
  name: include
  type: array
provider_name: APIs.io
provider_slug: apis-io
schema_file: json-schema/apis-io-search-ap-is-json-schema.json
slug: apis-io-search-ap-is-json
source_filename: apis-io-search-ap-is-json-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-ap-is-json-schema.json\",\n  \"title\": \"APIsJSON\",\n  \"description\": \"APIsJSON schema from APIs.io Search API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"description\",\n    \"url\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service described\",\n      \"minLength\": 5\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the service\",\n      \"minLength\": 5\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL where the apis.json file will live\",\n      \"pattern\": \"^(http)|(https)://(.*)$\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"Image to represent the API\"\n    },\n   \
  \ \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the file was created\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the file was modified\"\n    },\n    \"specificationVersion\": {\n      \"type\": \"string\",\n      \"description\": \"APIs.json spec version, latest is 0.18\",\n      \"enum\": [\n        0.18,\n        0.17,\n        0.16,\n        0.15,\n        0.14\n      ]\n    },\n    \"apis\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/API\"\n      },\n      \"description\": \"All the APIs of this service\"\n    },\n    \"maintainers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Maintainer\"\n      },\n      \"description\": \"Maintainers of the apis.json file\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  $ref\": \"#/components/schemas/Tag\"\n      },\n      \"description\": \"Tags to describe the service\"\n    },\n    \"include\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Include\"\n      },\n      \"description\": \"Links to other apis.json definitions included in this service.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-ap-is-json-schema.json
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
title: APIsJSON
---
