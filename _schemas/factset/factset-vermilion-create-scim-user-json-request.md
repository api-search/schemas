---
description: ''
layout: schema
name: CreateScimUserJSONRequest
properties_list:
- description: ''
  name: userName
  type: string
- description: ''
  name: password
  type: string
- description: ''
  name: name
  type: object
- description: ''
  name: preferredLanguage
  type: string
- description: ''
  name: active
  type: boolean
- description: ''
  name: authenticatedUserName
  type: string
- description: ''
  name: tenant
  type: string
- description: ''
  name: phoneNumbers
  type: array
- description: ''
  name: emails
  type: array
- description: ''
  name: photos
  type: array
- description: ''
  name: tenancies
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vermilion-create-scim-user-json-request-schema.json
slug: factset-vermilion-create-scim-user-json-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateScimUserJSONRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userName\": {\n      \"type\": \"string\"\n    },\n    \"password\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"object\"\n    },\n    \"preferredLanguage\": {\n      \"type\": \"string\"\n    },\n    \"active\": {\n      \"type\": \"boolean\"\n    },\n    \"authenticatedUserName\": {\n      \"type\": \"string\"\n    },\n    \"tenant\": {\n      \"type\": \"string\"\n    },\n    \"phoneNumbers\": {\n      \"type\": \"array\"\n    },\n    \"emails\": {\n      \"type\": \"array\"\n    },\n    \"photos\": {\n      \"type\": \"array\"\n    },\n    \"tenancies\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vermilion-create-scim-user-json-request-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CreateScimUserJSONRequest
---
