---
description: PaymentType schema from Adyen API
layout: schema
name: PaymentType
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-payment-type-schema.json
slug: terminal-payment-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-type-schema.json\",\n  \"title\": \"PaymentType\",\n  \"description\": \"PaymentType schema from Adyen API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CashAdvance\",\n    \"CashDeposit\",\n    \"Completion\",\n    \"FirstReservation\",\n    \"Instalment\",\n    \"IssuerInstalment\",\n    \"Normal\",\n    \"OneTimeReservation\",\n    \"PaidOut\",\n    \"Recurring\",\n    \"Refund\",\n    \"UpdateReservation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-type-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentType
---
