---
description: RepaymentTerm schema from Adyen API
layout: schema
name: RepaymentTerm
properties_list:
- description: The estimated term for repaying the grant, in days.
  name: estimatedDays
  type: integer
- description: The maximum term for repaying the grant, in days. Only applies when `contractType` is **loan**.
  name: maximumDays
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-repayment-term-schema.json
slug: configuration-repayment-term
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-repayment-term-schema.json\",\n  \"title\": \"RepaymentTerm\",\n  \"description\": \"RepaymentTerm schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"estimatedDays\": {\n      \"description\": \"The estimated term for repaying the grant, in days.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"maximumDays\": {\n      \"description\": \"The maximum term for repaying the grant, in days. Only applies when `contractType` is **loan**.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"estimatedDays\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-repayment-term-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RepaymentTerm
---
