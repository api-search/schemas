---
description: ''
layout: schema
name: ContactSummaryDto
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
  name: employerName
  type: string
- description: ''
  name: employerIdentifier
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: stateProvince
  type: string
- description: ''
  name: postalCode
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: isDeleted
  type: boolean
- description: ''
  name: lastMeeting
  type: string
- description: ''
  name: alternativeEmailAddresses
  type: array
- description: ''
  name: customFieldValues
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-contacts-contact-summary-dto-schema.json
slug: factset-irn-contacts-contact-summary-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactSummaryDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"primaryEmailAddress\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\"\n    },\n    \"fullName\": {\n      \"type\": \"string\"\n    },\n    \"employerName\": {\n      \"type\": \"string\"\n    },\n    \"employerIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"stateProvince\": {\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"isDeleted\": {\n      \"type\": \"boolean\"\n    },\n    \"lastMeeting\": {\n      \"type\": \"string\"\n    },\n    \"alternativeEmailAddresses\": {\n      \"type\": \"array\"\n    },\n    \"customFieldValues\": {\n      \"type\": \"array\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-contacts-contact-summary-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ContactSummaryDto
---
