---
description: TaxInformation schema from Adyen API
layout: schema
name: TaxInformation
properties_list:
- description: The two-letter [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code.
  name: country
  type: string
- description: The tax ID number (TIN) of the organization or individual.
  name: number
  type: string
- description: 'The TIN type depending on the country where it was issued. Provide only for countries that have multiple tax IDs, such as Sweden, the UK, or the US. For example, provide **SSN**, **EIN**, or **ITIN** '
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-tax-information-schema.json
slug: legal-entity-tax-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-tax-information-schema.json\",\n  \"title\": \"TaxInformation\",\n  \"description\": \"TaxInformation schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"country\": {\n      \"description\": \"The two-letter [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code.\",\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"number\": {\n      \"description\": \"The tax ID number (TIN) of the organization or individual.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The TIN type depending on the country where it was issued. Provide only for countries that have multiple tax IDs, such as Sweden, the UK, or the US. For example, provide **SSN**, **EIN**, or **ITIN** for the US.\",\n\
  \      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-tax-information-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TaxInformation
---
