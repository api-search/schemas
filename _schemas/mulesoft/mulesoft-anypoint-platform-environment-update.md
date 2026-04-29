---
description: Request body for updating an environment
layout: schema
name: EnvironmentUpdate
properties_list:
- description: New display name for the environment
  name: name
  type: string
- description: New environment type classification
  name: type
  type: string
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-environment-update-schema.json
slug: mulesoft-anypoint-platform-environment-update
source_filename: mulesoft-anypoint-platform-environment-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvironmentUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating an environment\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"New display name for the environment\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"New environment type classification\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-environment-update-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: EnvironmentUpdate
---
