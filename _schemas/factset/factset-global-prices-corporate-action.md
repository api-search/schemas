---
description: ''
layout: schema
name: corporateAction
properties_list:
- description: Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equit
  name: fsymId
  type: string
- description: FactSet identifier that uniquely identifies the Event.
  name: eventId
  type: string
- description: 'Corporate Actions Event type code, possible values: [ DVC, DVCD, DRP, DVS, DVSS, BNS, BNSS, SPO, DSR, FSP, RSP, SPL ]'
  name: eventTypeCode
  type: string
- description: Corporate Actions Event type description.
  name: eventTypeDesc
  type: string
- description: 'Dividend Type Code. For code descriptions, visit [Online Assistant Page #8764] (https://oa.apps.factset.com/pages/8764).'
  name: divTypeCode
  type: string
- description: Date Event was announced in YYYY-MM-DD format.
  name: announcementDate
  type: string
- description: Date of Record for distribution in YYYY-MM-DD format.
  name: recordDate
  type: string
- description: Date of Payment for distribution in YYYY-MM-DD format.
  name: payDate
  type: string
- description: Effective Date or Ex-Date of distribution in YYYY-MM-DD format.
  name: effectiveDate
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-prices-corporate-action-schema.json
slug: factset-global-prices-corporate-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"corporateAction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equities, all primary listings per region and currency are allocated a regional-level permanent identifier. The regional-level permanent identifier will be available once a SEDOL representing the region/currency has been allocated and the identifiers are on FactSet.\"\n    },\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet identifier that uniquely identifies the Event.\"\n    },\n    \"eventTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"Corporate Actions Event type code, possible values: [ DVC, DVCD, DRP, DVS,\
  \ DVSS, BNS, BNSS, SPO, DSR, FSP, RSP, SPL ]\"\n    },\n    \"eventTypeDesc\": {\n      \"type\": \"string\",\n      \"description\": \"Corporate Actions Event type description.\"\n    },\n    \"divTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"Dividend Type Code. For code descriptions, visit [Online Assistant Page #8764] (https://oa.apps.factset.com/pages/8764).\\n\"\n    },\n    \"announcementDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date Event was announced in YYYY-MM-DD format.\"\n    },\n    \"recordDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of Record for distribution in YYYY-MM-DD format.\"\n    },\n    \"payDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of Payment for distribution in YYYY-MM-DD format.\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"Effective Date or Ex-Date of distribution in YYYY-MM-DD format.\"\n    },\n    \"requestId\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-prices-corporate-action-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: corporateAction
---
