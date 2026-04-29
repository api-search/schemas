---
description: HTTP endpoint data source configuration
layout: schema
name: HttpDataSourceConfig
properties_list:
- description: HTTP endpoint URL
  name: endpoint
  type: string
- description: Authorization configuration for the HTTP endpoint
  name: authorizationConfig
  type: object
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-http-data-source-config-schema.json
slug: appsync-http-data-source-config
source_filename: appsync-http-data-source-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-http-data-source-config-schema.json\",\n  \"title\": \"HttpDataSourceConfig\",\n  \"description\": \"HTTP endpoint data source configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP endpoint URL\"\n    },\n    \"authorizationConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Authorization configuration for the HTTP endpoint\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-http-data-source-config-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: HttpDataSourceConfig
---
