---
description: ''
layout: schema
name: UserInfo
properties_list:
- description: Account type (user or organization)
  name: type
  type: string
- description: ''
  name: id
  type: string
- description: Username
  name: name
  type: string
- description: Full display name
  name: fullname
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: emailVerified
  type: boolean
- description: Subscription plan
  name: plan
  type: string
- description: ''
  name: canPay
  type: boolean
- description: ''
  name: avatarUrl
  type: string
- description: ''
  name: orgs
  type: array
- description: ''
  name: auth
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-hub-user-info-schema.json
slug: hugging-face-hub-user-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Account type (user or organization)\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Username\"\n    },\n    \"fullname\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"emailVerified\": {\n      \"type\": \"boolean\"\n    },\n    \"plan\": {\n      \"type\": \"string\",\n      \"description\": \"Subscription plan\"\n    },\n    \"canPay\": {\n      \"type\": \"boolean\"\n    },\n    \"avatarUrl\": {\n      \"type\": \"string\"\n    },\n    \"orgs\": {\n      \"type\": \"array\"\n    },\n    \"auth\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-hub-user-info-schema.json
tags: []
title: UserInfo
---
