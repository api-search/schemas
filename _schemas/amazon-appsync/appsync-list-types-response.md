---
description: Response with list of types
layout: schema
name: ListTypesResponse
properties_list:
- description: List of types
  name: types
  type: array
- description: Pagination token
  name: nextToken
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-list-types-response-schema.json
slug: appsync-list-types-response
source_filename: appsync-list-types-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-list-types-response-schema.json\",\n  \"title\": \"ListTypesResponse\",\n  \"description\": \"Response with list of types\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"types\": {\n      \"type\": \"array\",\n      \"description\": \"List of types\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-list-types-response-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: ListTypesResponse
---
