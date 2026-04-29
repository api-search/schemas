---
description: PackageSearchResponse schema from Ballerina Central API
layout: schema
name: PackageSearchResponse
properties_list:
- description: ''
  name: packages
  type: array
- description: Total number of matching packages
  name: count
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: limit
  type: integer
provider_name: Ballerina
provider_slug: ballerina
schema_file: json-schema/central-api-package-search-response-schema.json
slug: central-api-package-search-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-package-search-response-schema.json\",\n  \"title\": \"PackageSearchResponse\",\n  \"description\": \"PackageSearchResponse schema from Ballerina Central API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"packages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PackageSummary\"\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching packages\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-package-search-response-schema.json
tags:
- Integrations
- Orchestrations
- Open Source
- Programming Language
title: PackageSearchResponse
---
