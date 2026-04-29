---
description: Organization schema from Ballerina Central API
layout: schema
name: Organization
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: website
  type: string
- description: ''
  name: packageCount
  type: integer
provider_name: Ballerina
provider_slug: ballerina
schema_file: json-schema/central-api-organization-schema.json
slug: central-api-organization
source_filename: central-api-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-organization-schema.json\",\n  \"title\": \"Organization\",\n  \"description\": \"Organization schema from Ballerina Central API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"packageCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/json-schema/central-api-organization-schema.json
tags:
- Integrations
- Orchestrations
- Open Source
- Programming Language
title: Organization
---
