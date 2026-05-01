---
description: Represents an attribute for describing the schema for a table or index
layout: schema
name: AttributeDefinition
properties_list:
- description: A name for the attribute
  name: AttributeName
  type: string
- description: The data type for the attribute
  name: AttributeType
  type: string
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/dynamodb-openapi-attribute-definition-schema.json
slug: dynamodb-openapi-attribute-definition
source_filename: dynamodb-openapi-attribute-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-attribute-definition-schema.json\",\n  \"title\": \"AttributeDefinition\",\n  \"description\": \"Represents an attribute for describing the schema for a table or index\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttributeName\": {\n      \"type\": \"string\",\n      \"description\": \"A name for the attribute\"\n    },\n    \"AttributeType\": {\n      \"type\": \"string\",\n      \"description\": \"The data type for the attribute\",\n      \"enum\": [\n        \"S\",\n        \"N\",\n        \"B\"\n      ]\n    }\n  },\n  \"required\": [\n    \"AttributeName\",\n    \"AttributeType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/dynamodb-openapi-attribute-definition-schema.json
tags:
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: AttributeDefinition
---
