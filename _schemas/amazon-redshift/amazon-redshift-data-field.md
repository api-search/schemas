---
description: A single value in a result row. Exactly one of the typed properties will be present, corresponding to the column data type.
layout: schema
name: Field
properties_list:
- description: A value in binary format
  name: blobValue
  type: string
- description: A boolean value
  name: booleanValue
  type: boolean
- description: A double-precision floating point value
  name: doubleValue
  type: number
- description: Whether the value is null
  name: isNull
  type: boolean
- description: A long integer value
  name: longValue
  type: integer
- description: A string value
  name: stringValue
  type: string
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-data-field-schema.json
slug: amazon-redshift-data-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Field\",\n  \"type\": \"object\",\n  \"description\": \"A single value in a result row. Exactly one of the typed properties will be present, corresponding to the column data type.\",\n  \"properties\": {\n    \"blobValue\": {\n      \"type\": \"string\",\n      \"description\": \"A value in binary format\"\n    },\n    \"booleanValue\": {\n      \"type\": \"boolean\",\n      \"description\": \"A boolean value\"\n    },\n    \"doubleValue\": {\n      \"type\": \"number\",\n      \"description\": \"A double-precision floating point value\"\n    },\n    \"isNull\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the value is null\"\n    },\n    \"longValue\": {\n      \"type\": \"integer\",\n      \"description\": \"A long integer value\"\n    },\n    \"stringValue\": {\n      \"type\": \"string\",\n      \"description\": \"A string value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-data-field-schema.json
tags:
- Analytics
- Big Data
- Cloud
- Data Lake
- Data Warehouse
- ETL
- Machine Learning
- Serverless
- SQL
title: Field
---
