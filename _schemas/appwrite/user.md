---
description: An Appwrite user account with authentication credentials
layout: schema
name: User
properties_list:
- description: Unique user identifier
  name: $id
  type: string
- description: User display name
  name: name
  type: string
- description: User email address
  name: email
  type: string
- description: User phone number
  name: phone
  type: string
- description: Whether email is verified
  name: emailVerification
  type: boolean
- description: Whether phone is verified
  name: phoneVerification
  type: boolean
- description: User account status (active/disabled)
  name: status
  type: boolean
- description: Account creation timestamp
  name: createdAt
  type: string
- description: Last update timestamp
  name: updatedAt
  type: string
- description: User labels for RBAC
  name: labels
  type: array
provider_name: Appwrite
provider_slug: appwrite
schema_file: json-schema/user-schema.json
slug: user
source_filename: user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appwrite/main/json-schema/user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"An Appwrite user account with authentication credentials\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"$id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique user identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User display name\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"User email address\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"User phone number\"\n    },\n    \"emailVerification\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether email is verified\"\n    },\n    \"phoneVerification\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether phone\
  \ is verified\"\n    },\n    \"status\": {\n      \"type\": \"boolean\",\n      \"description\": \"User account status (active/disabled)\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Account creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User labels for RBAC\"\n    }\n  },\n  \"required\": [\n    \"$id\",\n    \"email\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appwrite/refs/heads/main/json-schema/user-schema.json
tags:
- Applications
- Backends
- Mobile
- Open Source
title: User
---
