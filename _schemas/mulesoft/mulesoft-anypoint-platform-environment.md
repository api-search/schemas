---
description: A deployment environment within an organization. Environments provide isolated contexts for deploying Mule applications, with types including Design, Sandbox, and Production.
layout: schema
name: Environment
properties_list:
- description: Unique identifier of the environment
  name: id
  type: string
- description: Display name of the environment
  name: name
  type: string
- description: ID of the organization this environment belongs to
  name: organizationId
  type: string
- description: Whether this is a production environment
  name: isProduction
  type: boolean
- description: The environment type classification
  name: type
  type: string
- description: Client ID associated with this environment
  name: clientId
  type: string
- description: Timestamp when the environment was created
  name: createdAt
  type: string
- description: Timestamp when the environment was last updated
  name: updatedAt
  type: string
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-environment-schema.json
slug: mulesoft-anypoint-platform-environment
source_filename: mulesoft-anypoint-platform-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Environment\",\n  \"type\": \"object\",\n  \"description\": \"A deployment environment within an organization. Environments provide isolated contexts for deploying Mule applications, with types including Design, Sandbox, and Production.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the environment\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the environment\"\n    },\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the organization this environment belongs to\"\n    },\n    \"isProduction\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a production environment\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The environment type classification\"\n    },\n    \"clientId\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"Client ID associated with this environment\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the environment was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the environment was last updated\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-environment-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: Environment
---
