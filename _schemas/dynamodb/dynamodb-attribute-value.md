---
description: Represents the data for an attribute. Each attribute value is described as a name-value pair. The name is the data type, and the value is the data itself. DynamoDB supports scalar types (String, Number, Binary, Boolean, Null), document types (List, Map), and set types (String Set, Number Set, Binary Set).
layout: schema
name: AttributeValue
properties_list:
- description: An attribute of type String
  name: S
  type: string
- description: An attribute of type Number (sent as a string to preserve precision)
  name: N
  type: string
- description: An attribute of type Binary (Base64-encoded)
  name: B
  type: string
- description: An attribute of type String Set
  name: SS
  type: array
- description: An attribute of type Number Set
  name: NS
  type: array
- description: An attribute of type Binary Set
  name: BS
  type: array
- description: An attribute of type Map
  name: M
  type: object
- description: An attribute of type List
  name: L
  type: array
- description: An attribute of type Null
  name: 'NULL'
  type: boolean
- description: An attribute of type Boolean
  name: BOOL
  type: boolean
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-attribute-value-schema.json
slug: dynamodb-attribute-value
source_filename: dynamodb-attribute-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AttributeValue\",\n  \"type\": \"object\",\n  \"description\": \"Represents the data for an attribute. Each attribute value is described as a name-value pair. The name is the data type, and the value is the data itself. DynamoDB supports scalar types (String, Number, Binary, Boolean, Null), document types (List, Map), and set types (String Set, Number Set, Binary Set).\",\n  \"properties\": {\n    \"S\": {\n      \"type\": \"string\",\n      \"description\": \"An attribute of type String\"\n    },\n    \"N\": {\n      \"type\": \"string\",\n      \"description\": \"An attribute of type Number (sent as a string to preserve precision)\"\n    },\n    \"B\": {\n      \"type\": \"string\",\n      \"description\": \"An attribute of type Binary (Base64-encoded)\"\n    },\n    \"SS\": {\n      \"type\": \"array\",\n      \"description\": \"An attribute of type String Set\"\n    },\n    \"NS\": {\n \
  \     \"type\": \"array\",\n      \"description\": \"An attribute of type Number Set\"\n    },\n    \"BS\": {\n      \"type\": \"array\",\n      \"description\": \"An attribute of type Binary Set\"\n    },\n    \"M\": {\n      \"type\": \"object\",\n      \"description\": \"An attribute of type Map\"\n    },\n    \"L\": {\n      \"type\": \"array\",\n      \"description\": \"An attribute of type List\"\n    },\n    \"NULL\": {\n      \"type\": \"boolean\",\n      \"description\": \"An attribute of type Null\"\n    },\n    \"BOOL\": {\n      \"type\": \"boolean\",\n      \"description\": \"An attribute of type Boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-attribute-value-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: AttributeValue
---
