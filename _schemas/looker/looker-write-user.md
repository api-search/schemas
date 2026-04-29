---
description: Writable fields for creating or updating a user
layout: schema
name: WriteUser
properties_list:
- description: First name
  name: first_name
  type: string
- description: Last name
  name: last_name
  type: string
- description: Email address
  name: email
  type: string
- description: Whether the account is disabled
  name: is_disabled
  type: boolean
- description: Locale setting
  name: locale
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-write-user-schema.json
slug: looker-write-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WriteUser\",\n  \"type\": \"object\",\n  \"description\": \"Writable fields for creating or updating a user\",\n  \"properties\": {\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address\"\n    },\n    \"is_disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account is disabled\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"Locale setting\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-write-user-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: WriteUser
---
