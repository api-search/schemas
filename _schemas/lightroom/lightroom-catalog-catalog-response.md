---
description: ''
layout: schema
name: CatalogResponse
properties_list:
- description: Base URL for the API
  name: base
  type: string
- description: Unique catalog identifier
  name: id
  type: string
- description: Resource type
  name: type
  type: string
- description: Server-side creation timestamp
  name: created
  type: string
- description: Server-side last updated timestamp
  name: updated
  type: string
- description: Catalog metadata
  name: payload
  type: object
- description: HATEOAS links to related resources
  name: links
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-catalog-catalog-response-schema.json
slug: lightroom-catalog-catalog-response
source_filename: lightroom-catalog-catalog-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CatalogResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"base\": {\n      \"type\": \"string\",\n      \"description\": \"Base URL for the API\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique catalog identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"Server-side creation timestamp\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"description\": \"Server-side last updated timestamp\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Catalog metadata\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS links to related resources\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-catalog-catalog-response-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: CatalogResponse
---
