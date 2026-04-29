---
description: Set a value or values for a custom field identified by the field 'Code'. Only one of the fields (IntegerValue / TextValue / FilePathValue etc) will be used, depending on the data type of the custom field corresponding to the 'Code' provided
layout: schema
name: CreateCustomFieldValueDto
properties_list:
- description: ''
  name: code
  type: string
- description: ''
  name: integerValue
  type: integer
- description: ''
  name: textValue
  type: string
- description: ''
  name: filePathValue
  type: string
- description: ''
  name: numericValue
  type: number
- description: ''
  name: dateValue
  type: string
- description: ''
  name: extendedTextValue
  type: string
- description: ''
  name: contactLookupValues
  type: array
- description: ''
  name: optionValue
  type: string
- description: ''
  name: optionValues
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-notes-create-custom-field-value-dto-schema.json
slug: factset-irn-notes-create-custom-field-value-dto
source_filename: factset-irn-notes-create-custom-field-value-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateCustomFieldValueDto\",\n  \"type\": \"object\",\n  \"description\": \"Set a value or values for a custom field identified by the field 'Code'. Only one of the fields (IntegerValue / TextValue / FilePathValue etc) will be used,\\r\\ndepending on the data type of the custom field corresponding to the 'Code' provided\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"integerValue\": {\n      \"type\": \"integer\"\n    },\n    \"textValue\": {\n      \"type\": \"string\"\n    },\n    \"filePathValue\": {\n      \"type\": \"string\"\n    },\n    \"numericValue\": {\n      \"type\": \"number\"\n    },\n    \"dateValue\": {\n      \"type\": \"string\"\n    },\n    \"extendedTextValue\": {\n      \"type\": \"string\"\n    },\n    \"contactLookupValues\": {\n      \"type\": \"array\"\n    },\n    \"optionValue\": {\n      \"type\": \"string\"\n    },\n    \"optionValues\"\
  : {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-notes-create-custom-field-value-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CreateCustomFieldValueDto
---
