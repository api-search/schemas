---
description: ''
layout: schema
name: SanctionScreening
properties_list:
- description: Known as VAT Number in the US and GST in Canada.
  name: taxId
  type: string
- description: The merchant's former legal names
  name: formerLegalNames
  type: array
- description: Indicates whether the merchant does business with sanctioned geographies. If it is true, then sanctionedGeographies property can't be empty.
  name: doBusinessWithSanctionedGeographies
  type: boolean
- description: List of sanctioned geographies that the merchant is doing business with. It can't be empty if the doBusinessWithSanctionedGeographies property is true
  name: sanctionedGeographies
  type: array
- description: Indicates whether a merchant is publicly traded.
  name: publiclyTraded
  type: boolean
- description: Publicly traded merchant's stock symbol. It's mandatory if the isPubliclyTraded attribute is true.
  name: tickerSymbol
  type: string
- description: Required only if publiclyTraded property is false and legalEntities property is empty.
  name: beneficialOwners
  type: array
- description: Required only if publiclyTraded property is false and beneficialOwners property is empty.
  name: legalEntities
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-sanction-screening-schema.json
slug: mastercard-ethoca-merchant-self-services-sanction-screening
source_filename: mastercard-ethoca-merchant-self-services-sanction-screening-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SanctionScreening\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taxId\": {\n      \"type\": \"string\",\n      \"description\": \"Known as VAT Number in the US and GST in Canada.\"\n    },\n    \"formerLegalNames\": {\n      \"type\": \"array\",\n      \"description\": \"The merchant's former legal names\"\n    },\n    \"doBusinessWithSanctionedGeographies\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the merchant does business with sanctioned geographies.\\nIf it is true, then sanctionedGeographies property can't be empty.\\n\"\n    },\n    \"sanctionedGeographies\": {\n      \"type\": \"array\",\n      \"description\": \"List of sanctioned geographies that the merchant is doing business with. It\\ncan't be empty if the doBusinessWithSanctionedGeographies property is true\\n\"\n    },\n    \"publiclyTraded\": {\n      \"type\": \"boolean\",\n     \
  \ \"description\": \"Indicates whether a merchant is publicly traded.\"\n    },\n    \"tickerSymbol\": {\n      \"type\": \"string\",\n      \"description\": \"Publicly traded merchant's stock symbol. It's mandatory if the isPubliclyTraded attribute is true.\"\n    },\n    \"beneficialOwners\": {\n      \"type\": \"array\",\n      \"description\": \"Required only if publiclyTraded property is false and legalEntities property is empty.\"\n    },\n    \"legalEntities\": {\n      \"type\": \"array\",\n      \"description\": \"Required only if publiclyTraded property is false and beneficialOwners property is empty.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-sanction-screening-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: SanctionScreening
---
