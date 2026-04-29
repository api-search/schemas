---
description: ''
layout: schema
name: TableField
properties_list:
- description: Unique identifier for a combination of table and data field
  name: id
  type: string
- description: Unique identifier for the data item
  name: dataItemId
  type: string
- description: Name of the data field
  name: name
  type: string
- description: Data type of the data field
  name: dataType
  type: string
- description: Column position of the data field within the table
  name: position
  type: integer
- description: Flag indicating if the data field is a primary key.
  name: isPrimaryKey
  type: boolean
- description: Flag indicating if a data field is nullable
  name: nullable
  type: boolean
- description: Flag indicating if the field's value is determined by a code value in its row. The monetary, splitAffected and unitFactor fields for that value will also be inherited from the code.
  name: hasCodeDependency
  type: boolean
- description: Flag indicating if the data field contained in this TableField is monetary. If true, this field can have exchange rates applied to convert to other currencies
  name: monetary
  type: boolean
- description: Flag indicating if the data field contained in this TableField can be affected by splits
  name: splitAffected
  type: boolean
- description: Factor to indicate what units that the data field is displayed in. If null, the field does not need to have a factor applied to obtain the real value
  name: unitFactor
  type: string
- description: A description of the data field within the context of its table
  name: description
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-content-feeds-data-dictionary-table-field-schema.json
slug: factset-content-feeds-data-dictionary-table-field
source_filename: factset-content-feeds-data-dictionary-table-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableField\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for a combination of table and data field\"\n    },\n    \"dataItemId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the data item\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the data field\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"description\": \"Data type of the data field\"\n    },\n    \"position\": {\n      \"type\": \"integer\",\n      \"description\": \"Column position of the data field within the table\"\n    },\n    \"isPrimaryKey\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if the data field is a primary key.\"\n    },\n    \"nullable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag\
  \ indicating if a data field is nullable\"\n    },\n    \"hasCodeDependency\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if the field's value is determined by a code value in its row. The monetary, splitAffected and unitFactor fields for that value will also be inherited from the code.\"\n    },\n    \"monetary\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if the data field contained in this TableField is monetary. If true, this field can have exchange rates applied to convert to other currencies\"\n    },\n    \"splitAffected\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if the data field contained in this TableField can be affected by splits\"\n    },\n    \"unitFactor\": {\n      \"type\": \"string\",\n      \"description\": \"Factor to indicate what units that the data field is displayed in. If null, the field does not need to have a factor applied to obtain the real value\"\n    },\n    \"\
  description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the data field within the context of its table\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-content-feeds-data-dictionary-table-field-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: TableField
---
