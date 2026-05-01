---
description: Response with list of GraphQL APIs
layout: schema
name: ListGraphqlApisResponse
properties_list:
- description: List of GraphQL APIs
  name: graphqlApis
  type: array
- description: Pagination token
  name: nextToken
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-list-graphql-apis-response-schema.json
slug: appsync-list-graphql-apis-response
source_filename: appsync-list-graphql-apis-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-list-graphql-apis-response-schema.json\",\n  \"title\": \"ListGraphqlApisResponse\",\n  \"description\": \"Response with list of GraphQL APIs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphqlApis\": {\n      \"type\": \"array\",\n      \"description\": \"List of GraphQL APIs\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-list-graphql-apis-response-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: ListGraphqlApisResponse
---
