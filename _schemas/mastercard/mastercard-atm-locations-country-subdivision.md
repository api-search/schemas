---
description: Available information the Country Subdivision such as the name and code
layout: schema
name: CountrySubdivision
properties_list:
- description: Abbreviated code for the state or province
  name: countrySubdivisionCode
  type: string
- description: Name of the country subdivision
  name: countrySubdivisionName
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-atm-locations-country-subdivision-schema.json
slug: mastercard-atm-locations-country-subdivision
source_filename: mastercard-atm-locations-country-subdivision-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CountrySubdivision\",\n  \"type\": \"object\",\n  \"description\": \"Available information the Country Subdivision such as the name and code\",\n  \"properties\": {\n    \"countrySubdivisionCode\": {\n      \"type\": \"string\",\n      \"description\": \"Abbreviated code for the state or province\"\n    },\n    \"countrySubdivisionName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the country subdivision\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-atm-locations-country-subdivision-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CountrySubdivision
---
