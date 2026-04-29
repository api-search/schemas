---
description: In the Payment or the Loyalty Request message, it allows to identify the loyalty account by the Sale Terminal instead of the POI Terminal (e.g. because the account identification is a bar-code read by the Cashier on a scanner device). Identification of a Loyalty account.
layout: schema
name: LoyaltyAccountID
properties_list:
- description: ''
  name: EntryMode
  type: object
- description: ''
  name: IdentificationType
  type: object
- description: ''
  name: IdentificationSupport
  type: object
- description: ''
  name: LoyaltyID
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-loyalty-account-id-schema.json
slug: terminal-loyalty-account-id
source_filename: terminal-loyalty-account-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-account-id-schema.json\",\n  \"title\": \"LoyaltyAccountID\",\n  \"description\": \"In the Payment or the Loyalty Request message, it allows to identify the loyalty account by the Sale Terminal instead of the POI Terminal (e.g. because the account identification is a bar-code read by the Cashier on a scanner device). Identification of a Loyalty account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntryMode\": {\n      \"$ref\": \"#/components/schemas/EntryMode\"\n    },\n    \"IdentificationType\": {\n      \"$ref\": \"#/components/schemas/IdentificationType\"\n    },\n    \"IdentificationSupport\": {\n      \"$ref\": \"#/components/schemas/IdentificationSupport\"\n    },\n    \"LoyaltyID\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"EntryMode\",\n    \"IdentificationType\"\
  ,\n    \"LoyaltyID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-account-id-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoyaltyAccountID
---
