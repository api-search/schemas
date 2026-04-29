---
description: PackageSummary schema from Ballerina Central API
layout: schema
name: PackageSummary
properties_list:
- description: ''
  name: organization
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: platform
  type: string
- description: ''
  name: ballerinaVersion
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: pullCount
  type: integer
- description: ''
  name: createdDate
  type: string
- description: ''
  name: keywords
  type: array
- description: ''
  name: license
  type: string
- description: ''
  name: authors
  type: array
provider_name: Ballerina
provider_slug: ballerina
schema_file: json-schema/central-api-package-summary-schema.json
slug: central-api-package-summary
source_filename: central-api-package-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-package-summary-schema.json\",\n  \"title\": \"PackageSummary\",\n  \"description\": \"PackageSummary schema from Ballerina Central API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organization\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"platform\": {\n      \"type\": \"string\"\n    },\n    \"ballerinaVersion\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"pullCount\": {\n      \"type\": \"integer\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"keywords\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n\
  \    \"license\": {\n      \"type\": \"string\"\n    },\n    \"authors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-package-summary-schema.json
tags:
- Integrations
- Orchestrations
- Open Source
- Programming Language
title: PackageSummary
---
