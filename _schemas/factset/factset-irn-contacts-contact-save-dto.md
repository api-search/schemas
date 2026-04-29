---
description: ''
layout: schema
name: ContactSaveDto
properties_list:
- description: ''
  name: primaryEmailAddress
  type: string
- description: ''
  name: fullName
  type: string
- description: ''
  name: notes
  type: string
- description: ''
  name: linkedInProfile
  type: string
- description: ''
  name: personSymbol
  type: string
- description: ''
  name: roleId
  type: string
- description: ''
  name: typeId
  type: string
- description: ''
  name: phoneNumbers
  type: array
- description: ''
  name: leftRelationships
  type: array
- description: ''
  name: rightRelationships
  type: array
- description: ''
  name: alternativeEmailAddresses
  type: array
- description: ''
  name: customFields
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-contacts-contact-save-dto-schema.json
slug: factset-irn-contacts-contact-save-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactSaveDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"primaryEmailAddress\": {\n      \"type\": \"string\"\n    },\n    \"fullName\": {\n      \"type\": \"string\"\n    },\n    \"notes\": {\n      \"type\": \"string\"\n    },\n    \"linkedInProfile\": {\n      \"type\": \"string\"\n    },\n    \"personSymbol\": {\n      \"type\": \"string\"\n    },\n    \"roleId\": {\n      \"type\": \"string\"\n    },\n    \"typeId\": {\n      \"type\": \"string\"\n    },\n    \"phoneNumbers\": {\n      \"type\": \"array\"\n    },\n    \"leftRelationships\": {\n      \"type\": \"array\"\n    },\n    \"rightRelationships\": {\n      \"type\": \"array\"\n    },\n    \"alternativeEmailAddresses\": {\n      \"type\": \"array\"\n    },\n    \"customFields\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-contacts-contact-save-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ContactSaveDto
---
