---
description: It conveys Information related to the status of the last or current Payment, Loyalty or Reversal transaction. Content of the TransactionStatus Response message.
layout: schema
name: TransactionStatusResponse
properties_list:
- description: ''
  name: Response
  type: object
- description: ''
  name: MessageReference
  type: object
- description: ''
  name: RepeatedMessageResponse
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-transaction-status-response-schema.json
slug: terminal-transaction-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-status-response-schema.json\",\n  \"title\": \"TransactionStatusResponse\",\n  \"description\": \"It conveys Information related to the status of the last or current Payment, Loyalty or Reversal transaction. Content of the TransactionStatus Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"MessageReference\": {\n      \"$ref\": \"#/components/schemas/MessageReference\"\n    },\n    \"RepeatedMessageResponse\": {\n      \"$ref\": \"#/components/schemas/RepeatedMessageResponse\"\n    }\n  },\n  \"required\": [\n    \"Response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-status-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionStatusResponse
---
