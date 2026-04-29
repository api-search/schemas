---
description: A custom field value for a catalog object
layout: schema
name: CustomFieldValue
properties_list:
- description: ''
  name: field_id
  type: integer
- description: ''
  name: field_name
  type: string
- description: ''
  name: object_type
  type: string
- description: ''
  name: object_id
  type: integer
- description: Field value
  name: value
  type: object
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-data-catalog-custom-field-value-schema.json
slug: alation-alation-data-catalog-custom-field-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-data-catalog-custom-field-value-schema.json\",\n  \"title\": \"CustomFieldValue\",\n  \"description\": \"A custom field value for a catalog object\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field_id\": {\n      \"type\": \"integer\"\n    },\n    \"field_name\": {\n      \"type\": \"string\"\n    },\n    \"object_type\": {\n      \"type\": \"string\"\n    },\n    \"object_id\": {\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"description\": \"Field value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-data-catalog-custom-field-value-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: CustomFieldValue
---
