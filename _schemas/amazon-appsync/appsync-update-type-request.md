---
description: Request to update a type
layout: schema
name: UpdateTypeRequest
properties_list:
- description: The updated type definition
  name: definition
  type: string
- description: The definition format
  name: format
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-update-type-request-schema.json
slug: appsync-update-type-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-update-type-request-schema.json\",\n  \"title\": \"UpdateTypeRequest\",\n  \"description\": \"Request to update a type\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"definition\": {\n      \"type\": \"string\",\n      \"description\": \"The updated type definition\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"The definition format\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-update-type-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: UpdateTypeRequest
---
