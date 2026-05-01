---
description: Represents the data for an attribute. Each attribute value is described as a name-value pair with the data type as the name.
layout: schema
name: AttributeValue
properties_list:
- description: String attribute value
  name: S
  type: string
- description: Number attribute value (sent as string)
  name: N
  type: string
- description: Binary attribute value (Base64-encoded)
  name: B
  type: string
- description: String set attribute value
  name: SS
  type: array
- description: Number set attribute value
  name: NS
  type: array
- description: Binary set attribute value
  name: BS
  type: array
- description: Map attribute value
  name: M
  type: object
- description: List attribute value
  name: L
  type: array
- description: Null attribute value
  name: 'NULL'
  type: boolean
- description: Boolean attribute value
  name: BOOL
  type: boolean
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-attribute-value-schema.json
slug: dynamodb-openapi-attribute-value
source_filename: dynamodb-openapi-attribute-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-attribute-value-schema.json\",\n  \"title\": \"AttributeValue\",\n  \"description\": \"Represents the data for an attribute. Each attribute value is described as a name-value pair with the data type as the name.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S\": {\n      \"type\": \"string\",\n      \"description\": \"String attribute value\"\n    },\n    \"N\": {\n      \"type\": \"string\",\n      \"description\": \"Number attribute value (sent as string)\"\n    },\n    \"B\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"description\": \"Binary attribute value (Base64-encoded)\"\n    },\n    \"SS\": {\n      \"type\": \"array\",\n      \"description\": \"String set attribute value\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n\
  \    \"NS\": {\n      \"type\": \"array\",\n      \"description\": \"Number set attribute value\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"BS\": {\n      \"type\": \"array\",\n      \"description\": \"Binary set attribute value\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"byte\"\n      }\n    },\n    \"M\": {\n      \"type\": \"object\",\n      \"description\": \"Map attribute value\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    },\n    \"L\": {\n      \"type\": \"array\",\n      \"description\": \"List attribute value\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AttributeValue\"\n      }\n    },\n    \"NULL\": {\n      \"type\": \"boolean\",\n      \"description\": \"Null attribute value\"\n    },\n    \"BOOL\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean attribute value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-attribute-value-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: AttributeValue
---
