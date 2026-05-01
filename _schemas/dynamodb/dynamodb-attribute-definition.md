---
description: ''
layout: schema
name: AttributeDefinition
properties_list:
- description: A name for the attribute
  name: AttributeName
  type: string
- description: 'The data type for the attribute: S (String), N (Number), B (Binary)'
  name: AttributeType
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-attribute-definition-schema.json
slug: dynamodb-attribute-definition
source_filename: dynamodb-attribute-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AttributeDefinition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttributeName\": {\n      \"type\": \"string\",\n      \"description\": \"A name for the attribute\"\n    },\n    \"AttributeType\": {\n      \"type\": \"string\",\n      \"description\": \"The data type for the attribute: S (String), N (Number), B (Binary)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-attribute-definition-schema.json
tags:
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: AttributeDefinition
---
