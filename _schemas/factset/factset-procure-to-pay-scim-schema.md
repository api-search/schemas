---
description: ''
layout: schema
name: Schema
properties_list:
- description: The unique URI of the schema. When applicable, service providers MUST specify the URI.
  name: id
  type: string
- description: The schema's human-readable name. When applicable, service providers MUST specify the name, e.g., 'User'.
  name: name
  type: string
- description: The schema's human-readable name. When applicable, service providers MUST specify the name, e.g., 'User'.
  name: description
  type: string
- description: A complex attribute that includes the attributes of a schema.
  name: attributes
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-procure-to-pay-scim-schema-schema.json
slug: factset-procure-to-pay-scim-schema
source_filename: factset-procure-to-pay-scim-schema-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique URI of the schema. When applicable, service providers MUST specify the URI.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The schema's human-readable name.  When applicable, service providers MUST specify the name, e.g., 'User'.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The schema's human-readable name.  When applicable, service providers MUST specify the name, e.g., 'User'.\"\n    },\n    \"attributes\": {\n      \"type\": \"array\",\n      \"description\": \"A complex attribute that includes the attributes of a schema.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-procure-to-pay-scim-schema-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Schema
---
