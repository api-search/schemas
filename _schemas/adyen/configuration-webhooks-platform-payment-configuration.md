---
description: PlatformPaymentConfiguration schema from Adyen API
layout: schema
name: PlatformPaymentConfiguration
properties_list:
- description: 'Specifies at what time a [sales day](https://docs.adyen.com/marketplaces-and-platforms/settle-funds/sales-day-settlement#sales-day) ends. Possible values: Time in **"HH:MM"** format. **HH** ranges fro'
  name: salesDayClosingTime
  type: string
- description: Specifies after how many business days the funds in a [settlement batch](https://docs.adyen.com/marketplaces-and-platforms/settle-funds/sales-day-settlement#settlement-batch) are made available. Possi
  name: settlementDelayDays
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-platform-payment-configuration-schema.json
slug: configuration-webhooks-platform-payment-configuration
source_filename: configuration-webhooks-platform-payment-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-platform-payment-configuration-schema.json\",\n  \"title\": \"PlatformPaymentConfiguration\",\n  \"description\": \"PlatformPaymentConfiguration schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"salesDayClosingTime\": {\n      \"description\": \"Specifies at what time a [sales day](https://docs.adyen.com/marketplaces-and-platforms/settle-funds/sales-day-settlement#sales-day) ends.\\n\\nPossible values: Time in **\\\"HH:MM\\\"** format. **HH** ranges from **00** to **07**. **MM** must be **00**.\\n\\nDefault value: **\\\"00:00\\\"**.\",\n      \"format\": \"time\",\n      \"type\": \"string\"\n    },\n    \"settlementDelayDays\": {\n      \"description\": \"Specifies after how many business days the funds in a [settlement batch](https://docs.adyen.com/marketplaces-and-platforms/settle-funds/sales-day-settlement#settlement-batch)\
  \ are made available.\\n\\nPossible values: **0** to **10**, or **null**.\\n* Setting this value to an integer enables [Sales day settlement](https://docs.adyen.com/marketplaces-and-platforms/settle-funds/sales-day-settlement).\\n* Setting this value to **null** enables [Pass-through settlement](https://docs.adyen.com/marketplaces-and-platforms/settle-funds/pass-through-settlement).\\n\\nDefault value: **null**.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-platform-payment-configuration-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PlatformPaymentConfiguration
---
