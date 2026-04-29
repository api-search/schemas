---
description: ''
layout: schema
name: ContactDto
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: primaryEmailAddress
  type: string
- description: ''
  name: identifier
  type: string
- description: ''
  name: fullName
  type: string
- description: ''
  name: linkedInProfile
  type: string
- description: ''
  name: isDeleted
  type: boolean
- description: ''
  name: phoneNumbers
  type: array
- description: ''
  name: alternativeEmailAddresses
  type: array
- description: ''
  name: customFields
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-contacts-contact-dto-schema.json
slug: factset-irn-contacts-contact-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"primaryEmailAddress\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\"\n    },\n    \"fullName\": {\n      \"type\": \"string\"\n    },\n    \"linkedInProfile\": {\n      \"type\": \"string\"\n    },\n    \"isDeleted\": {\n      \"type\": \"boolean\"\n    },\n    \"phoneNumbers\": {\n      \"type\": \"array\"\n    },\n    \"alternativeEmailAddresses\": {\n      \"type\": \"array\"\n    },\n    \"customFields\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-contacts-contact-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ContactDto
---
