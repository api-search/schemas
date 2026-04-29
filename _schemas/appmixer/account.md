---
description: An Account represents an authenticated connection to a third-party service (e.g. OAuth credentials for Slack, Google, etc.) belonging to an Appmixer user.
layout: schema
name: Appmixer Account
properties_list:
- description: Unique identifier for the connected account.
  name: accountId
  type: string
- description: Display name for the connected account.
  name: name
  type: string
- description: The service or connector this account is associated with (e.g. appmixer.google).
  name: service
  type: string
- description: Profile information retrieved from the third-party service.
  name: profileInfo
  type: object
- description: Whether the account credentials (tokens) are still valid.
  name: valid
  type: boolean
provider_name: Appmixer
provider_slug: appmixer
schema_file: json-schema/account.json
slug: account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/appmixer/blob/main/json-schema/account.json\",\n  \"title\": \"Appmixer Account\",\n  \"description\": \"An Account represents an authenticated connection to a third-party service (e.g. OAuth credentials for Slack, Google, etc.) belonging to an Appmixer user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the connected account.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the connected account.\"\n    },\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"The service or connector this account is associated with (e.g. appmixer.google).\"\n    },\n    \"profileInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Profile information retrieved from the third-party service.\",\n\
  \      \"additionalProperties\": true\n    },\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account credentials (tokens) are still valid.\"\n    }\n  },\n  \"required\": [\"accountId\", \"service\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/json-schema/account.json
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
title: Appmixer Account
---
