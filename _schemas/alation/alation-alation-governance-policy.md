---
description: A data governance policy
layout: schema
name: Policy
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: policy_type
  type: string
- description: ''
  name: stewards
  type: array
- description: ''
  name: url
  type: string
- description: ''
  name: created_at
  type: string
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-governance-policy-schema.json
slug: alation-alation-governance-policy
source_filename: alation-alation-governance-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-governance-policy-schema.json\",\n  \"title\": \"Policy\",\n  \"description\": \"A data governance policy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"policy_type\": {\n      \"type\": \"string\"\n    },\n    \"stewards\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-governance-policy-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: Policy
---
