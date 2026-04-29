---
description: StoredDetails schema from Adyen API
layout: schema
name: StoredDetails
properties_list:
- description: The stored bank account.
  name: bank
  type: object
- description: The stored card information.
  name: card
  type: object
- description: The email associated with stored payment details.
  name: emailAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-stored-details-schema.json
slug: checkout-stored-details
source_filename: checkout-stored-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-stored-details-schema.json\",\n  \"title\": \"StoredDetails\",\n  \"description\": \"StoredDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bank\": {\n      \"description\": \"The stored bank account.\",\n      \"$ref\": \"#/components/schemas/BankAccount\"\n    },\n    \"card\": {\n      \"description\": \"The stored card information.\",\n      \"$ref\": \"#/components/schemas/Card\"\n    },\n    \"emailAddress\": {\n      \"description\": \"The email associated with stored payment details.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-stored-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredDetails
---
