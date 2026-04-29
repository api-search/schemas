---
description: NetworkToken schema from Adyen API
layout: schema
name: NetworkToken
properties_list:
- description: The card brand variant of the payment instrument associated with the network token. For example, **mc_prepaid_mrw**.
  name: brandVariant
  type: string
- description: Date and time when the network token was created, in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) extended format. For example, **2020-12-18T10:15:30+01:00**..
  name: creationDate
  type: string
- description: Device details.
  name: device
  type: object
- description: The unique identifier of the network token.
  name: id
  type: string
- description: The unique identifier of the payment instrument to which this network token belongs to.
  name: paymentInstrumentId
  type: string
- description: 'The status of the network token. Possible values: **active**, **inactive**, **suspended**, **closed**.'
  name: status
  type: string
- description: The last four digits of the network token `id`.
  name: tokenLastFour
  type: string
- description: The type of wallet the network token is associated with. For example, **applePay**.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-network-token-schema.json
slug: configuration-network-token
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-network-token-schema.json\",\n  \"title\": \"NetworkToken\",\n  \"description\": \"NetworkToken schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brandVariant\": {\n      \"description\": \"The card brand variant of the payment instrument associated with the network token. For example, **mc_prepaid_mrw**.\",\n      \"type\": \"string\"\n    },\n    \"creationDate\": {\n      \"description\": \"Date and time when the network token was created, in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) extended format. For example, **2020-12-18T10:15:30+01:00**..\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"device\": {\n      \"description\": \"Device details.\",\n      \"$ref\": \"#/components/schemas/DeviceInfo\"\n    },\n  \
  \  \"id\": {\n      \"description\": \"The unique identifier of the network token.\",\n      \"type\": \"string\"\n    },\n    \"paymentInstrumentId\": {\n      \"description\": \"The unique identifier of the payment instrument to which this network token belongs to.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the network token. Possible values: **active**, **inactive**, **suspended**, **closed**.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"suspended\",\n        \"closed\"\n      ],\n      \"type\": \"string\"\n    },\n    \"tokenLastFour\": {\n      \"description\": \"The last four digits of the network token `id`.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of wallet the network token is associated with. For example, **applePay**.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-network-token-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NetworkToken
---
