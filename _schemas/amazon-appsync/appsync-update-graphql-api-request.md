---
description: Request to update a GraphQL API
layout: schema
name: UpdateGraphqlApiRequest
properties_list:
- description: The API name
  name: name
  type: string
- description: Authentication type
  name: authenticationType
  type: string
- description: logConfig
  name: logConfig
  type: string
- description: Enable X-Ray tracing
  name: xrayEnabled
  type: boolean
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-update-graphql-api-request-schema.json
slug: appsync-update-graphql-api-request
source_filename: appsync-update-graphql-api-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-update-graphql-api-request-schema.json\",\n  \"title\": \"UpdateGraphqlApiRequest\",\n  \"description\": \"Request to update a GraphQL API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The API name\"\n    },\n    \"authenticationType\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication type\"\n    },\n    \"logConfig\": {\n      \"type\": \"string\",\n      \"description\": \"logConfig\"\n    },\n    \"xrayEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable X-Ray tracing\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-update-graphql-api-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: UpdateGraphqlApiRequest
---
