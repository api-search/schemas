---
description: Convertible Details for a Fixed Income security.
layout: schema
name: convertibleDetails
properties_list:
- description: Security identifier used in the request.
  name: requestId
  type: string
- description: FactSet Permanent Security Identifier.
  name: fsymId
  type: string
- description: Convertible Currency
  name: convCurr
  type: string
- description: Convertible Effective Date
  name: convEffDate
  type: string
- description: Convertible End Date
  name: convEndDate
  type: string
- description: Convertible Frequency
  name: convFrequency
  type: string
- description: Convertible Type Id
  name: convId
  type: integer
- description: Convertible Identification
  name: convIdentification
  type: string
- description: Convertible Notice Max
  name: convNoticeDaysMax
  type: integer
- description: Convertible Notice Min
  name: convNoticeDaysMin
  type: integer
- description: Convertible Payment Form
  name: convPayForm
  type: string
- description: Convertible Payment Form Detail
  name: convPayFormDet
  type: string
- description: Convertible Payment Form Election
  name: convPayFormElect
  type: string
- description: Convertible Premium Change Control
  name: convPremChgControl
  type: number
- description: Convertible Price Method
  name: convPriceMethod
  type: string
- description: Convertibles Ratio
  name: convRatio
  type: number
- description: Convertible Ratio Form Description
  name: convRatioDesc
  type: string
- description: Convertible Type
  name: convType
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-convertible-details-schema.json
slug: factset-terms-and-conditions-convertible-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"convertibleDetails\",\n  \"type\": \"object\",\n  \"description\": \"Convertible Details for a Fixed Income security.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier used in the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Permanent Security Identifier.\"\n    },\n    \"convCurr\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Currency\"\n    },\n    \"convEffDate\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Effective Date\"\n    },\n    \"convEndDate\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible End Date\"\n    },\n    \"convFrequency\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Frequency\"\n    },\n    \"convId\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Convertible Type Id\"\n    },\n    \"convIdentification\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Identification\"\n    },\n    \"convNoticeDaysMax\": {\n      \"type\": \"integer\",\n      \"description\": \"Convertible Notice Max\"\n    },\n    \"convNoticeDaysMin\": {\n      \"type\": \"integer\",\n      \"description\": \"Convertible Notice Min\"\n    },\n    \"convPayForm\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Payment Form\"\n    },\n    \"convPayFormDet\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Payment Form Detail\"\n    },\n    \"convPayFormElect\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Payment Form Election\"\n    },\n    \"convPremChgControl\": {\n      \"type\": \"number\",\n      \"description\": \"Convertible Premium Change Control\"\n    },\n    \"convPriceMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Price Method\"\
  \n    },\n    \"convRatio\": {\n      \"type\": \"number\",\n      \"description\": \"Convertibles Ratio\"\n    },\n    \"convRatioDesc\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Ratio Form Description\"\n    },\n    \"convType\": {\n      \"type\": \"string\",\n      \"description\": \"Convertible Type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-convertible-details-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: convertibleDetails
---
