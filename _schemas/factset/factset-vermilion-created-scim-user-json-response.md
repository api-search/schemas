---
description: ''
layout: schema
name: CreatedScimUserJSONResponse
properties_list:
- description: ''
  name: schemas
  type: array
- description: ''
  name: id
  type: integer
- description: ''
  name: userName
  type: string
- description: ''
  name: name
  type: object
- description: ''
  name: userType
  type: string
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
  name: tenancies
  type: array
- description: ''
  name: photos
  type: array
- description: ''
  name: domainCode
  type: string
- description: ''
  name: isAdministrator
  type: boolean
- description: ''
  name: meta
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-vermilion-created-scim-user-json-response-schema.json
slug: factset-vermilion-created-scim-user-json-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreatedScimUserJSONResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\"\n    },\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"userName\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"object\"\n    },\n    \"userType\": {\n      \"type\": \"string\"\n    },\n    \"preferredLanguage\": {\n      \"type\": \"string\"\n    },\n    \"active\": {\n      \"type\": \"boolean\"\n    },\n    \"authenticatedUserName\": {\n      \"type\": \"string\"\n    },\n    \"tenant\": {\n      \"type\": \"string\"\n    },\n    \"phoneNumbers\": {\n      \"type\": \"array\"\n    },\n    \"emails\": {\n      \"type\": \"array\"\n    },\n    \"tenancies\": {\n      \"type\": \"array\"\n    },\n    \"photos\": {\n      \"type\": \"array\"\n    },\n    \"domainCode\": {\n      \"type\": \"string\"\n    },\n    \"isAdministrator\"\
  : {\n      \"type\": \"boolean\"\n    },\n    \"meta\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-vermilion-created-scim-user-json-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CreatedScimUserJSONResponse
---
