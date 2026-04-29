---
description: CardHolderPIN schema from Adyen API
layout: schema
name: CardHolderPIN
properties_list:
- description: ''
  name: EncrPINBlock
  type: string
- description: ''
  name: PINFormat
  type: object
- description: ''
  name: AdditionalInput
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-card-holder-pin-schema.json
slug: terminal-card-holder-pin
source_filename: terminal-card-holder-pin-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-holder-pin-schema.json\",\n  \"title\": \"CardHolderPIN\",\n  \"description\": \"CardHolderPIN schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EncrPINBlock\": {\n      \"type\": \"string\"\n    },\n    \"PINFormat\": {\n      \"$ref\": \"#/components/schemas/PINFormat\"\n    },\n    \"AdditionalInput\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    }\n  },\n  \"required\": [\n    \"EncrPINBlock\",\n    \"PINFormat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-holder-pin-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardHolderPIN
---
