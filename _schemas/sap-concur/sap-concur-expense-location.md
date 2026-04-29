---
description: A geographic location associated with an expense
layout: schema
name: Location
properties_list:
- description: The location identifier
  name: id
  type: string
- description: The localized location name
  name: name
  type: string
- description: The city name
  name: city
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: countryCode
  type: string
- description: ISO 3166-2 subdivision code
  name: countrySubDivisionCode
  type: string
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-location-schema.json
slug: sap-concur-expense-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Location\",\n  \"type\": \"object\",\n  \"description\": \"A geographic location associated with an expense\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The location identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The localized location name\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city name\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\"\n    },\n    \"countrySubDivisionCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-2 subdivision code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-location-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: Location
---
