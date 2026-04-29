---
description: Request to start schema creation
layout: schema
name: StartSchemaCreationRequest
properties_list:
- description: The new schema definition in SDL format
  name: definition
  type: string
provider_name: Amazon AppSync
provider_slug: amazon-appsync
schema_file: json-schema/appsync-start-schema-creation-request-schema.json
slug: appsync-start-schema-creation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-appsync/json-schema/appsync-start-schema-creation-request-schema.json\",\n  \"title\": \"StartSchemaCreationRequest\",\n  \"description\": \"Request to start schema creation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"definition\": {\n      \"type\": \"string\",\n      \"description\": \"The new schema definition in SDL format\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appsync/refs/heads/main/json-schema/appsync-start-schema-creation-request-schema.json
tags:
- Amazon AppSync
- GraphQL
- API Management
- Serverless
- AWS
title: StartSchemaCreationRequest
---
