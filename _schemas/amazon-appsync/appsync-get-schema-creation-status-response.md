---
description: Response with schema creation status
layout: schema
name: GetSchemaCreationStatusResponse
properties_list:
- description: Schema creation status
  name: status
  type: string
- description: Status details
  name: details
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-get-schema-creation-status-response-schema.json
slug: appsync-get-schema-creation-status-response
source_filename: appsync-get-schema-creation-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-get-schema-creation-status-response-schema.json\",\n  \"title\": \"GetSchemaCreationStatusResponse\",\n  \"description\": \"Response with schema creation status\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Schema creation status\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Status details\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-get-schema-creation-status-response-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
title: GetSchemaCreationStatusResponse
---
