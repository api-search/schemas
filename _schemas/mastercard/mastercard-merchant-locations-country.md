---
description: Available information for the Country such as the name and code
layout: schema
name: Country
properties_list:
- description: Three digit alpha country code as defined in ISO 3166-1
  name: countryCode
  type: string
- description: Name of the country
  name: countryName
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-merchant-locations-country-schema.json
slug: mastercard-merchant-locations-country
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Country\",\n  \"type\": \"object\",\n  \"description\": \"Available information for the Country such as the name and code\",\n  \"properties\": {\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Three digit alpha country code as defined in ISO 3166-1\"\n    },\n    \"countryName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the country\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-merchant-locations-country-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Country
---
