---
description: Payload for creating a new user.
layout: schema
name: UserCreate
properties_list:
- description: The name of the user.
  name: name
  type: string
- description: The user's email address.
  name: email
  type: string
- description: The user's phone number.
  name: phone
  type: string
- description: ''
  name: role
  type: string
- description: ''
  name: custom_role_id
  type: integer
- description: ''
  name: organization_id
  type: integer
- description: ''
  name: external_id
  type: string
- description: ''
  name: tags
  type: array
- description: ''
  name: locale_id
  type: integer
- description: ''
  name: time_zone
  type: string
- description: ''
  name: details
  type: string
- description: ''
  name: notes
  type: string
- description: ''
  name: alias
  type: string
- description: ''
  name: signature
  type: string
- description: ''
  name: verified
  type: boolean
- description: ''
  name: user_fields
  type: object
provider_name: Zendesk
provider_slug: zendesk
schema_file: json-schema/zendesk-support-user-create-schema.json
slug: zendesk-support-user-create
source_filename: zendesk-support-user-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserCreate\",\n  \"type\": \"object\",\n  \"description\": \"Payload for creating a new user.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The user's email address.\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"The user's phone number.\"\n    },\n    \"role\": {\n      \"type\": \"string\"\n    },\n    \"custom_role_id\": {\n      \"type\": \"integer\"\n    },\n    \"organization_id\": {\n      \"type\": \"integer\"\n    },\n    \"external_id\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"locale_id\": {\n      \"type\": \"integer\"\n    },\n    \"time_zone\": {\n      \"type\": \"string\"\n    },\n    \"details\": {\n      \"type\": \"string\"\n    },\n\
  \    \"notes\": {\n      \"type\": \"string\"\n    },\n    \"alias\": {\n      \"type\": \"string\"\n    },\n    \"signature\": {\n      \"type\": \"string\"\n    },\n    \"verified\": {\n      \"type\": \"boolean\"\n    },\n    \"user_fields\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zendesk/refs/heads/main/json-schema/zendesk-support-user-create-schema.json
tags:
- Chat
- CRM
- Help Center
- Sell
- Support
- T1
- Talk
- Ticketing
- Tickets
title: UserCreate
---
