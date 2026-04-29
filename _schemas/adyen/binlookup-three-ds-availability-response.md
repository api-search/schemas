---
description: ThreeDSAvailabilityResponse schema from Adyen API
layout: schema
name: ThreeDSAvailabilityResponse
properties_list:
- description: Bin Group Details
  name: binDetails
  type: object
- description: List of Directory Server (DS) public keys.
  name: dsPublicKeys
  type: array
- description: Indicator if 3D Secure 1 is supported.
  name: threeDS1Supported
  type: boolean
- description: List of brand and card range pairs.
  name: threeDS2CardRangeDetails
  type: array
- description: Indicator if 3D Secure 2 is supported.
  name: threeDS2supported
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/binlookup-three-ds-availability-response-schema.json
slug: binlookup-three-ds-availability-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-three-ds-availability-response-schema.json\",\n  \"title\": \"ThreeDSAvailabilityResponse\",\n  \"description\": \"ThreeDSAvailabilityResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"binDetails\": {\n      \"x-addedInVersion\": \"50\",\n      \"description\": \"Bin Group Details\",\n      \"$ref\": \"#/components/schemas/BinDetail\"\n    },\n    \"dsPublicKeys\": {\n      \"description\": \"List of Directory Server (DS) public keys.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DSPublicKeyDetail\"\n      },\n      \"type\": \"array\"\n    },\n    \"threeDS1Supported\": {\n      \"description\": \"Indicator if 3D Secure 1 is supported.\",\n      \"type\": \"boolean\"\n    },\n    \"threeDS2CardRangeDetails\": {\n      \"description\": \"List of brand\
  \ and card range pairs.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ThreeDS2CardRangeDetail\"\n      },\n      \"type\": \"array\"\n    },\n    \"threeDS2supported\": {\n      \"description\": \"Indicator if 3D Secure 2 is supported.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-three-ds-availability-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDSAvailabilityResponse
---
