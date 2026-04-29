---
description: RepeatedResponseMessageBody schema from Adyen API
layout: schema
name: RepeatedResponseMessageBody
properties_list:
- description: ''
  name: LoyaltyResponse
  type: object
- description: ''
  name: PaymentResponse
  type: object
- description: ''
  name: ReversalResponse
  type: object
- description: ''
  name: StoredValueResponse
  type: object
- description: ''
  name: CardAcquisitionResponse
  type: object
- description: ''
  name: CardReaderAPDUResponse
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-repeated-response-message-body-schema.json
slug: terminal-repeated-response-message-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-repeated-response-message-body-schema.json\",\n  \"title\": \"RepeatedResponseMessageBody\",\n  \"description\": \"RepeatedResponseMessageBody schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoyaltyResponse\": {\n      \"$ref\": \"#/components/schemas/LoyaltyResponse\"\n    },\n    \"PaymentResponse\": {\n      \"$ref\": \"#/components/schemas/PaymentResponse\"\n    },\n    \"ReversalResponse\": {\n      \"$ref\": \"#/components/schemas/ReversalResponse\"\n    },\n    \"StoredValueResponse\": {\n      \"$ref\": \"#/components/schemas/StoredValueResponse\"\n    },\n    \"CardAcquisitionResponse\": {\n      \"$ref\": \"#/components/schemas/CardAcquisitionResponse\"\n    },\n    \"CardReaderAPDUResponse\": {\n      \"$ref\": \"#/components/schemas/CardReaderAPDUResponse\"\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-repeated-response-message-body-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RepeatedResponseMessageBody
---
