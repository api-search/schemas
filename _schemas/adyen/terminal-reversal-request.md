---
description: It conveys Information related to the reversal of a previous payment or a loyalty transaction. Content of the Reversal Request message.
layout: schema
name: ReversalRequest
properties_list:
- description: ''
  name: SaleData
  type: object
- description: ''
  name: OriginalPOITransaction
  type: object
- description: ReversedAmount is implicitely the AuthorizedAmount if absent.
  name: ReversedAmount
  type: number
- description: ''
  name: ReversalReason
  type: object
- description: ''
  name: CustomerOrder
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-reversal-request-schema.json
slug: terminal-reversal-request
source_filename: terminal-reversal-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-reversal-request-schema.json\",\n  \"title\": \"ReversalRequest\",\n  \"description\": \"It conveys Information related to the reversal of a previous payment or a loyalty transaction. Content of the Reversal Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SaleData\": {\n      \"$ref\": \"#/components/schemas/SaleData\"\n    },\n    \"OriginalPOITransaction\": {\n      \"$ref\": \"#/components/schemas/OriginalPOITransaction\"\n    },\n    \"ReversedAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"ReversedAmount is implicitely the AuthorizedAmount if absent.\"\n    },\n    \"ReversalReason\": {\n      \"$ref\": \"#/components/schemas/ReversalReason\"\n    },\n    \"CustomerOrder\": {\n      \"$ref\": \"\
  #/components/schemas/CustomerOrder\"\n    }\n  },\n  \"required\": [\n    \"OriginalPOITransaction\",\n    \"ReversalReason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-reversal-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReversalRequest
---
