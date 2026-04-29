---
description: ''
layout: schema
name: SubjectConfigDto
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: code
  type: string
- description: ''
  name: isHidden
  type: boolean
- description: ''
  name: identifierType
  type: string
- description: ''
  name: identifierTypes
  type: array
- description: ''
  name: type
  type: string
- description: ''
  name: customFieldIds
  type: array
- description: ''
  name: newsHeadlineFormat
  type: array
- description: ''
  name: emailHeadlineFormat
  type: array
- description: ''
  name: noteLengthLimit
  type: integer
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-configuration-subject-config-dto-schema.json
slug: factset-irn-configuration-subject-config-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubjectConfigDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"isHidden\": {\n      \"type\": \"boolean\"\n    },\n    \"identifierType\": {\n      \"type\": \"string\"\n    },\n    \"identifierTypes\": {\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"customFieldIds\": {\n      \"type\": \"array\"\n    },\n    \"newsHeadlineFormat\": {\n      \"type\": \"array\"\n    },\n    \"emailHeadlineFormat\": {\n      \"type\": \"array\"\n    },\n    \"noteLengthLimit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-configuration-subject-config-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: SubjectConfigDto
---
