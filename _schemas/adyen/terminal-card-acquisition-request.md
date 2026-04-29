---
description: It conveys Information related to the payment and loyalty cards to read and analyse. This message pair is usually followed by a message pair (e.g. payment or loyalty) which refers to this Card Acquisition message pair. Content of the Card Acquisition Request message.
layout: schema
name: CardAcquisitionRequest
properties_list:
- description: ''
  name: SaleData
  type: object
- description: ''
  name: CardAcquisitionTransaction
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-card-acquisition-request-schema.json
slug: terminal-card-acquisition-request
source_filename: terminal-card-acquisition-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-acquisition-request-schema.json\",\n  \"title\": \"CardAcquisitionRequest\",\n  \"description\": \"It conveys Information related to the payment and loyalty cards to read and analyse. This message pair is usually followed by a message pair (e.g. payment or loyalty) which refers to this Card Acquisition message pair. Content of the Card Acquisition Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SaleData\": {\n      \"$ref\": \"#/components/schemas/SaleData\"\n    },\n    \"CardAcquisitionTransaction\": {\n      \"$ref\": \"#/components/schemas/CardAcquisitionTransaction\"\n    }\n  },\n  \"required\": [\n    \"SaleData\",\n    \"CardAcquisitionTransaction\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-acquisition-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardAcquisitionRequest
---
