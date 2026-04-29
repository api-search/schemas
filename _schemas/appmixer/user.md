---
description: A User represents an authenticated account in the Appmixer platform with access to flows, files, data stores, and connected third-party accounts.
layout: schema
name: Appmixer User
properties_list:
- description: Unique identifier for the user.
  name: id
  type: string
- description: The user's username, typically an email address.
  name: username
  type: string
- description: The user's email address.
  name: email
  type: string
- description: Authentication token for the user session.
  name: token
  type: string
- description: The subscription plan associated with the user.
  name: plan
  type: string
provider_name: Appmixer
provider_slug: appmixer
schema_file: json-schema/user.json
slug: user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/appmixer/blob/main/json-schema/user.json\",\n  \"title\": \"Appmixer User\",\n  \"description\": \"A User represents an authenticated account in the Appmixer platform with access to flows, files, data stores, and connected third-party accounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The user's username, typically an email address.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The user's email address.\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication token for the user session.\"\n    },\n    \"plan\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The subscription plan associated with the user.\"\n    }\n  },\n  \"required\": [\"id\", \"username\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/json-schema/user.json
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
title: Appmixer User
---
