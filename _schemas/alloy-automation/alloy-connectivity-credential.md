---
description: A stored credential for a user's connector
layout: schema
name: Credential
properties_list:
- description: Unique identifier for the credential
  name: credentialId
  type: string
- description: Connector this credential belongs to
  name: connectorId
  type: string
- description: User this credential belongs to
  name: userId
  type: string
- description: Timestamp when the credential was created
  name: createdAt
  type: string
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-credential-schema.json
slug: alloy-connectivity-credential
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-credential-schema.json\",\n  \"title\": \"Credential\",\n  \"type\": \"object\",\n  \"description\": \"A stored credential for a user's connector\",\n  \"properties\": {\n    \"credentialId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the credential\"\n    },\n    \"connectorId\": {\n      \"type\": \"string\",\n      \"description\": \"Connector this credential belongs to\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"User this credential belongs to\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the credential was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-credential-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: Credential
---
