---
description: Request body for creating a new environment
layout: schema
name: EnvironmentCreate
properties_list:
- description: Display name for the new environment
  name: name
  type: string
- description: The environment type classification
  name: type
  type: string
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-environment-create-schema.json
slug: mulesoft-anypoint-platform-environment-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvironmentCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new environment\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the new environment\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The environment type classification\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-environment-create-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: EnvironmentCreate
---
