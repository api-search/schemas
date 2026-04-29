---
description: Response with list of resolvers
layout: schema
name: ListResolversResponse
properties_list:
- description: List of resolvers
  name: resolvers
  type: array
- description: Pagination token
  name: nextToken
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-list-resolvers-response-schema.json
slug: appsync-list-resolvers-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-list-resolvers-response-schema.json\",\n  \"title\": \"ListResolversResponse\",\n  \"description\": \"Response with list of resolvers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resolvers\": {\n      \"type\": \"array\",\n      \"description\": \"List of resolvers\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-list-resolvers-response-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: ListResolversResponse
---
