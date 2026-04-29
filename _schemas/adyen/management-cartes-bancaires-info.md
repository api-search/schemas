---
description: CartesBancairesInfo schema from Adyen API
layout: schema
name: CartesBancairesInfo
properties_list:
- description: 'Cartes Bancaires SIRET. Format: 14 digits.'
  name: siret
  type: string
- description: Information regarding the transaction description.
  name: transactionDescription
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-cartes-bancaires-info-schema.json
slug: management-cartes-bancaires-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-cartes-bancaires-info-schema.json\",\n  \"title\": \"CartesBancairesInfo\",\n  \"description\": \"CartesBancairesInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"siret\": {\n      \"description\": \"Cartes Bancaires SIRET. Format: 14 digits.\",\n      \"type\": \"string\"\n    },\n    \"transactionDescription\": {\n      \"description\": \"Information regarding the transaction description.\",\n      \"$ref\": \"#/components/schemas/TransactionDescriptionInfo\"\n    }\n  },\n  \"required\": [\n    \"siret\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-cartes-bancaires-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CartesBancairesInfo
---
