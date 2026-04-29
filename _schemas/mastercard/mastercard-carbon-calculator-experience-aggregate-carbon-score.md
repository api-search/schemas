---
description: ''
layout: schema
name: AggregateCarbonScore
properties_list:
- description: An aggregate value of CO2 emission in grams.
  name: carbonEmissionInGrams
  type: string
- description: Denotes aggregate duration.
  name: aggregateDate
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-carbon-calculator-experience-aggregate-carbon-score-schema.json
slug: mastercard-carbon-calculator-experience-aggregate-carbon-score
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AggregateCarbonScore\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"carbonEmissionInGrams\": {\n      \"type\": \"string\",\n      \"description\": \"An aggregate value of CO2 emission in grams.\"\n    },\n    \"aggregateDate\": {\n      \"type\": \"string\",\n      \"description\": \"Denotes aggregate duration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-carbon-calculator-experience-aggregate-carbon-score-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AggregateCarbonScore
---
