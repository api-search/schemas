---
description: ''
layout: schema
name: CatalogResponse
properties_list:
- description: Base URL for the API
  name: base
  type: string
- description: Unique identifier of the catalog
  name: id
  type: string
- description: Resource type
  name: type
  type: string
- description: Catalog creation timestamp
  name: created
  type: string
- description: Catalog last updated timestamp
  name: updated
  type: string
- description: Catalog payload data
  name: payload
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-services-catalog-response-schema.json
slug: lightroom-services-catalog-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CatalogResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"base\": {\n      \"type\": \"string\",\n      \"description\": \"Base URL for the API\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the catalog\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"Catalog creation timestamp\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"description\": \"Catalog last updated timestamp\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Catalog payload data\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-services-catalog-response-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: CatalogResponse
---
