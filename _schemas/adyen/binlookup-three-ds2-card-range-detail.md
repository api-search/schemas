---
description: ThreeDS2CardRangeDetail schema from Adyen API
layout: schema
name: ThreeDS2CardRangeDetail
properties_list:
- description: 'Provides additional information to the 3DS Server. Possible values: - 01 (Authentication is available at ACS) - 02 (Attempts supported by ACS or DS) - 03 (Decoupled authentication supported) - 04 (Whi'
  name: acsInfoInd
  type: array
- description: Card brand.
  name: brandCode
  type: string
- description: BIN end range.
  name: endRange
  type: string
- description: BIN start range.
  name: startRange
  type: string
- description: Supported 3D Secure protocol versions
  name: threeDS2Versions
  type: array
- description: In a 3D Secure 2 browser-based flow, this is the URL where you should send the device fingerprint to.
  name: threeDSMethodURL
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/binlookup-three-ds2-card-range-detail-schema.json
slug: binlookup-three-ds2-card-range-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-three-ds2-card-range-detail-schema.json\",\n  \"title\": \"ThreeDS2CardRangeDetail\",\n  \"description\": \"ThreeDS2CardRangeDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acsInfoInd\": {\n      \"x-addedInVersion\": \"51\",\n      \"description\": \"Provides additional information to the 3DS Server.\\nPossible values:\\n- 01 (Authentication is available at ACS)\\n- 02 (Attempts supported by ACS or DS)\\n- 03 (Decoupled authentication supported)\\n- 04 (Whitelisting supported)\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"brandCode\": {\n      \"description\": \"Card brand.\",\n      \"type\": \"string\"\n    },\n    \"endRange\": {\n      \"description\": \"BIN end range.\",\n      \"type\": \"string\"\n \
  \   },\n    \"startRange\": {\n      \"description\": \"BIN start range.\",\n      \"type\": \"string\"\n    },\n    \"threeDS2Versions\": {\n      \"x-addedInVersion\": \"53\",\n      \"description\": \"Supported 3D Secure protocol versions\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"threeDSMethodURL\": {\n      \"description\": \"In a 3D Secure 2 browser-based flow, this is the URL where you should send the device fingerprint to.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-three-ds2-card-range-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDS2CardRangeDetail
---
