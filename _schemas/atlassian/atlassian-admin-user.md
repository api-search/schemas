---
description: Represents a user account in an Atlassian organization.
layout: schema
name: User
properties_list:
- description: The unique Atlassian account identifier.
  name: account_id
  type: string
- description: The type of account.
  name: account_type
  type: string
- description: The current status of the account.
  name: account_status
  type: string
- description: The display name of the user.
  name: name
  type: string
- description: The email address of the user.
  name: email
  type: string
- description: URL of the user's profile picture.
  name: picture
  type: string
- description: The nickname of the user.
  name: nickname
  type: string
- description: The last time the user was active.
  name: last_active
  type: string
- description: When the user account was created.
  name: created
  type: string
- description: Products the user has access to.
  name: product_access
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-user-schema.json
slug: atlassian-admin-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"Represents a user account in an Atlassian organization.\",\n  \"properties\": {\n    \"account_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Atlassian account identifier.\"\n    },\n    \"account_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of account.\"\n    },\n    \"account_status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the account.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the user.\"\n    },\n    \"picture\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the user's profile picture.\"\n    },\n    \"nickname\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"The nickname of the user.\"\n    },\n    \"last_active\": {\n      \"type\": \"string\",\n      \"description\": \"The last time the user was active.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"When the user account was created.\"\n    },\n    \"product_access\": {\n      \"type\": \"array\",\n      \"description\": \"Products the user has access to.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-user-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: User
---
