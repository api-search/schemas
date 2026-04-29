---
description: ChargePermission schema from Amazon Pay API
layout: schema
name: ChargePermission
properties_list:
- description: ''
  name: chargePermissionId
  type: string
- description: ''
  name: chargePermissionType
  type: string
- description: ''
  name: buyer
  type: object
- description: ''
  name: shippingAddress
  type: object
- description: ''
  name: billingAddress
  type: object
- description: ''
  name: statusDetails
  type: object
- description: ''
  name: limits
  type: object
- description: ''
  name: creationTimestamp
  type: string
- description: ''
  name: expirationTimestamp
  type: string
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/pay-charge-permission-schema.json
slug: pay-charge-permission
source_filename: pay-charge-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"chargePermissionId\": {\n      \"type\": \"string\"\n    },\n    \"chargePermissionType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OneTime\",\n        \"Recurring\"\n      ]\n    },\n    \"buyer\": {\n      \"$ref\": \"#/components/schemas/Buyer\"\n    },\n    \"shippingAddress\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"billingAddress\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"statusDetails\": {\n      \"$ref\": \"#/components/schemas/StatusDetails\"\n    },\n    \"limits\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amountLimit\": {\n          \"$ref\": \"#/components/schemas/Price\"\n        },\n        \"amountBalance\": {\n          \"$ref\": \"#/components/schemas/Price\"\n        }\n      }\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"expirationTimestamp\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChargePermission\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-charge-permission-schema.json\",\n  \"description\": \"ChargePermission schema from Amazon Pay API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/pay-charge-permission-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: ChargePermission
---
