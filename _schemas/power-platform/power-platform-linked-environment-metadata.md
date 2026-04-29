---
description: Metadata about the linked Dataverse instance.
layout: schema
name: LinkedEnvironmentMetadata
properties_list:
- description: The resource identifier of the Dataverse instance.
  name: resourceId
  type: string
- description: The friendly name of the Dataverse instance.
  name: friendlyName
  type: string
- description: The unique name identifier for the Dataverse organization.
  name: uniqueName
  type: string
- description: The domain name prefix for the Dataverse instance.
  name: domainName
  type: string
- description: The Dataverse platform version.
  name: version
  type: string
- description: The URL of the Dataverse instance.
  name: instanceUrl
  type: string
- description: The API URL for the Dataverse instance.
  name: instanceApiUrl
  type: string
- description: The LCID of the base language for the Dataverse instance.
  name: baseLanguage
  type: integer
- description: The state of the Dataverse instance.
  name: instanceState
  type: string
- description: The timestamp when the Dataverse instance was created.
  name: createdTime
  type: string
- description: Whether background operations are enabled.
  name: backgroundOperationsState
  type: string
- description: The scale group identifier.
  name: scaleGroup
  type: string
- description: The platform SKU of the Dataverse instance.
  name: platformSku
  type: string
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-linked-environment-metadata-schema.json
slug: power-platform-linked-environment-metadata
source_filename: power-platform-linked-environment-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LinkedEnvironmentMetadata\",\n  \"type\": \"['object', 'null']\",\n  \"description\": \"Metadata about the linked Dataverse instance.\",\n  \"properties\": {\n    \"resourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The resource identifier of the Dataverse instance.\"\n    },\n    \"friendlyName\": {\n      \"type\": \"string\",\n      \"description\": \"The friendly name of the Dataverse instance.\"\n    },\n    \"uniqueName\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name identifier for the Dataverse organization.\"\n    },\n    \"domainName\": {\n      \"type\": \"string\",\n      \"description\": \"The domain name prefix for the Dataverse instance.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The Dataverse platform version.\"\n    },\n    \"instanceUrl\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The URL of the Dataverse instance.\"\n    },\n    \"instanceApiUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The API URL for the Dataverse instance.\"\n    },\n    \"baseLanguage\": {\n      \"type\": \"integer\",\n      \"description\": \"The LCID of the base language for the Dataverse instance.\"\n    },\n    \"instanceState\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the Dataverse instance.\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the Dataverse instance was created.\"\n    },\n    \"backgroundOperationsState\": {\n      \"type\": \"string\",\n      \"description\": \"Whether background operations are enabled.\"\n    },\n    \"scaleGroup\": {\n      \"type\": \"string\",\n      \"description\": \"The scale group identifier.\"\n    },\n    \"platformSku\": {\n      \"type\": \"string\",\n      \"description\": \"The platform SKU of the Dataverse instance.\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-linked-environment-metadata-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: LinkedEnvironmentMetadata
---
