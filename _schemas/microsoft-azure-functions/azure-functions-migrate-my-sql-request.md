---
description: MySQL migration request.
layout: schema
name: MigrateMySqlRequest
properties_list:
- description: MigrateMySqlRequest resource specific properties
  name: properties
  type: object
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-migrate-my-sql-request-schema.json
slug: azure-functions-migrate-my-sql-request
source_filename: azure-functions-migrate-my-sql-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-migrate-my-sql-request-schema.json\",\n  \"title\": \"MigrateMySqlRequest\",\n  \"description\": \"MySQL migration request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/MigrateMySqlRequestProperties\",\n      \"description\": \"MigrateMySqlRequest resource specific properties\",\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-migrate-my-sql-request-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: MigrateMySqlRequest
---
