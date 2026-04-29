---
description: Request body for creating a connector credential
layout: schema
name: CreateCredentialRequest
properties_list:
- description: Identifier of the user
  name: userId
  type: string
- description: Connector-specific credential data
  name: data
  type: object
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-create_credential_request-schema.json
slug: alloy-connectivity-create_credential_request
source_filename: alloy-connectivity-create_credential_request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-create_credential_request-schema.json\",\n  \"title\": \"CreateCredentialRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a connector credential\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the user\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Connector-specific credential data\"\n    }\n  },\n  \"required\": [\n    \"userId\",\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-create_credential_request-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: CreateCredentialRequest
---
