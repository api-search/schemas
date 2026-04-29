---
description: Charge schema from Amazon Pay API
layout: schema
name: Charge
properties_list:
- description: ''
  name: chargeId
  type: string
- description: ''
  name: chargePermissionId
  type: string
- description: ''
  name: chargeAmount
  type: object
- description: ''
  name: captureAmount
  type: object
- description: ''
  name: refundedAmount
  type: object
- description: ''
  name: softDescriptor
  type: string
- description: ''
  name: statusDetails
  type: object
- description: ''
  name: creationTimestamp
  type: string
- description: ''
  name: expirationTimestamp
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/pay-charge-schema.json
slug: pay-charge
source_filename: pay-charge-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"chargeId\": {\n      \"type\": \"string\"\n    },\n    \"chargePermissionId\": {\n      \"type\": \"string\"\n    },\n    \"chargeAmount\": {\n      \"$ref\": \"#/components/schemas/Price\"\n    },\n    \"captureAmount\": {\n      \"$ref\": \"#/components/schemas/Price\"\n    },\n    \"refundedAmount\": {\n      \"$ref\": \"#/components/schemas/Price\"\n    },\n    \"softDescriptor\": {\n      \"type\": \"string\"\n    },\n    \"statusDetails\": {\n      \"$ref\": \"#/components/schemas/StatusDetails\"\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"expirationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Charge\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-charge-schema.json\"\
  ,\n  \"description\": \"Charge schema from Amazon Pay API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-charge-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: Charge
---
