---
description: Response with list of data sources
layout: schema
name: ListDataSourcesResponse
properties_list:
- description: List of data sources
  name: dataSources
  type: array
- description: Pagination token
  name: nextToken
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-list-data-sources-response-schema.json
slug: appsync-list-data-sources-response
source_filename: appsync-list-data-sources-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-list-data-sources-response-schema.json\",\n  \"title\": \"ListDataSourcesResponse\",\n  \"description\": \"Response with list of data sources\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataSources\": {\n      \"type\": \"array\",\n      \"description\": \"List of data sources\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-list-data-sources-response-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: ListDataSourcesResponse
---
