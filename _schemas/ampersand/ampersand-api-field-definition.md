---
description: Field definition for creating or updating custom fields
layout: schema
name: FieldDefinition
properties_list:
- description: The identifier of the field
  name: fieldName
  type: string
- description: The human-readable name of the field
  name: displayName
  type: string
- description: Optional description of the field
  name: description
  type: string
- description: The data type of the field. Valid values are string, boolean, date, datetime, singleSelect, multiSelect, int, float, reference
  name: valueType
  type: string
- description: Indicates if the field is required
  name: required
  type: boolean
- description: Indicates if the field must be unique across all records
  name: unique
  type: boolean
- description: Indicates if the field should be indexed for faster search
  name: indexed
  type: boolean
- description: ''
  name: stringOptions
  type: object
- description: ''
  name: numericOptions
  type: object
- description: ''
  name: association
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-field-definition-schema.json
slug: ampersand-api-field-definition
source_filename: ampersand-api-field-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-field-definition-schema.json\",\n  \"title\": \"FieldDefinition\",\n  \"description\": \"Field definition for creating or updating custom fields\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the field\",\n      \"example\": \"My_Custom_Field\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the field\",\n      \"example\": \"My Custom Field\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the field\"\n    },\n    \"valueType\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the field. Valid values are string, boolean, date, datetime, singleSelect,\
  \ multiSelect, int, float, reference\",\n      \"example\": \"string\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the field is required\"\n    },\n    \"unique\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the field must be unique across all records\"\n    },\n    \"indexed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the field should be indexed for faster search\"\n    },\n    \"stringOptions\": {\n      \"$ref\": \"#/components/schemas/StringFieldOptions\"\n    },\n    \"numericOptions\": {\n      \"$ref\": \"#/components/schemas/NumericFieldOptions\"\n    },\n    \"association\": {\n      \"$ref\": \"#/components/schemas/AssociationDefinition\"\n    }\n  },\n  \"required\": [\n    \"fieldName\",\n    \"displayName\",\n    \"valueType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-field-definition-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: FieldDefinition
---
