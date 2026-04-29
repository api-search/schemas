---
description: AdditionalCommission schema from Adyen API
layout: schema
name: AdditionalCommission
properties_list:
- description: Unique identifier of the balance account to which the additional commission is booked.
  name: balanceAccountId
  type: string
- description: A fixed commission fee, in minor units.
  name: fixedAmount
  type: integer
- description: A variable commission fee, in basis points.
  name: variablePercentage
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-additional-commission-schema.json
slug: management-additional-commission
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-additional-commission-schema.json\",\n  \"title\": \"AdditionalCommission\",\n  \"description\": \"AdditionalCommission schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balanceAccountId\": {\n      \"description\": \"Unique identifier of the balance account to which the additional commission is booked.\",\n      \"type\": \"string\"\n    },\n    \"fixedAmount\": {\n      \"description\": \"A fixed commission fee, in minor units.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"variablePercentage\": {\n      \"description\": \"A variable commission fee, in basis points.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-additional-commission-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalCommission
---
