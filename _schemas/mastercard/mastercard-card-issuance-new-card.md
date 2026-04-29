---
description: ''
layout: schema
name: NewCard
properties_list:
- description: Indicates whether number should be printed on the physical card or not. <BR/> Not applicable while issuing existing non-personalized card.
  name: numberless
  type: boolean
- description: Indicates whether instant card is required be generated or not. <BR/> It will be always considered as true in case of SVC/LVC card issuance irrespective of input value. <BR/>Not applicable while issui
  name: instant
  type: boolean
- description: Date on which card is delivered or handed over to client. <br/> Format - It is expressed in ISO 8601 - `YYYY-MM-DD`
  name: deliveryDate
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-new-card-schema.json
slug: mastercard-card-issuance-new-card
source_filename: mastercard-card-issuance-new-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NewCard\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"numberless\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether number should be printed on the physical card or not. <BR/> Not applicable while issuing existing non-personalized card.\"\n    },\n    \"instant\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether instant card is required be generated or not. <BR/> It will be always considered as true in case of SVC/LVC card issuance irrespective of input value. <BR/>Not applicable while issuing existing non-personalized card.\"\n    },\n    \"deliveryDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date on which card is delivered or handed over to client. <br/> Format - It is expressed in ISO 8601 - `YYYY-MM-DD`\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-new-card-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: NewCard
---
