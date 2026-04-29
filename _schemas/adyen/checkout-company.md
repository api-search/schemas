---
description: Company schema from Adyen API
layout: schema
name: Company
properties_list:
- description: The company website's home page.
  name: homepage
  type: string
- description: The company name.
  name: name
  type: string
- description: Registration number of the company.
  name: registrationNumber
  type: string
- description: Registry location of the company.
  name: registryLocation
  type: string
- description: Tax ID of the company.
  name: taxId
  type: string
- description: The company type.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-company-schema.json
slug: checkout-company
source_filename: checkout-company-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-company-schema.json\",\n  \"title\": \"Company\",\n  \"description\": \"Company schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"homepage\": {\n      \"description\": \"The company website's home page.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The company name.\",\n      \"type\": \"string\"\n    },\n    \"registrationNumber\": {\n      \"description\": \"Registration number of the company.\",\n      \"type\": \"string\"\n    },\n    \"registryLocation\": {\n      \"description\": \"Registry location of the company.\",\n      \"type\": \"string\"\n    },\n    \"taxId\": {\n      \"description\": \"Tax ID of the company.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The company type.\",\n      \"type\"\
  : \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-company-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Company
---
