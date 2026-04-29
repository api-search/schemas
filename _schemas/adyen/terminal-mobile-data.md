---
description: Mobile phone is used as a payment instrument for the transaction. Information related to the mobile for the payment transaction.
layout: schema
name: MobileData
properties_list:
- description: If data available.
  name: MobileCountryCode
  type: integer
- description: If data available.
  name: MobileNetworkCode
  type: integer
- description: If data available.
  name: MaskedMSISDN
  type: integer
- description: ''
  name: Geolocation
  type: object
- description: SensitiveMobileData.
  name: ProtectedMobileData
  type: string
- description: ''
  name: SensitiveMobileData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-mobile-data-schema.json
slug: terminal-mobile-data
source_filename: terminal-mobile-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-mobile-data-schema.json\",\n  \"title\": \"MobileData\",\n  \"description\": \"Mobile phone is used as a payment instrument for the transaction. Information related to the mobile for the payment transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MobileCountryCode\": {\n      \"type\": \"integer\",\n      \"minimum\": 3,\n      \"maximum\": 3,\n      \"description\": \"If data available.\"\n    },\n    \"MobileNetworkCode\": {\n      \"type\": \"integer\",\n      \"minimum\": 2,\n      \"maximum\": 3,\n      \"description\": \"If data available.\"\n    },\n    \"MaskedMSISDN\": {\n      \"type\": \"integer\",\n      \"description\": \"If data available.\"\n    },\n    \"Geolocation\": {\n      \"$ref\": \"#/components/schemas/Geolocation\"\n    },\n    \"ProtectedMobileData\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"SensitiveMobileData.\"\n    },\n    \"SensitiveMobileData\": {\n      \"$ref\": \"#/components/schemas/SensitiveMobileData\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-mobile-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MobileData
---
