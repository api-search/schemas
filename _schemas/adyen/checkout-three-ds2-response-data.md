---
description: ThreeDS2ResponseData schema from Adyen API
layout: schema
name: ThreeDS2ResponseData
properties_list:
- description: ''
  name: acsChallengeMandated
  type: string
- description: ''
  name: acsOperatorID
  type: string
- description: ''
  name: acsReferenceNumber
  type: string
- description: ''
  name: acsSignedContent
  type: string
- description: ''
  name: acsTransID
  type: string
- description: ''
  name: acsURL
  type: string
- description: ''
  name: authenticationType
  type: string
- description: ''
  name: cardHolderInfo
  type: string
- description: ''
  name: cavvAlgorithm
  type: string
- description: ''
  name: challengeIndicator
  type: string
- description: ''
  name: dsReferenceNumber
  type: string
- description: ''
  name: dsTransID
  type: string
- description: ''
  name: exemptionIndicator
  type: string
- description: ''
  name: messageVersion
  type: string
- description: ''
  name: riskScore
  type: string
- description: ''
  name: sdkEphemPubKey
  type: string
- description: ''
  name: threeDSServerTransID
  type: string
- description: ''
  name: transStatus
  type: string
- description: ''
  name: transStatusReason
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-three-ds2-response-data-schema.json
slug: checkout-three-ds2-response-data
source_filename: checkout-three-ds2-response-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-three-ds2-response-data-schema.json\",\n  \"title\": \"ThreeDS2ResponseData\",\n  \"description\": \"ThreeDS2ResponseData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acsChallengeMandated\": {\n      \"type\": \"string\"\n    },\n    \"acsOperatorID\": {\n      \"type\": \"string\"\n    },\n    \"acsReferenceNumber\": {\n      \"type\": \"string\"\n    },\n    \"acsSignedContent\": {\n      \"type\": \"string\"\n    },\n    \"acsTransID\": {\n      \"type\": \"string\"\n    },\n    \"acsURL\": {\n      \"type\": \"string\"\n    },\n    \"authenticationType\": {\n      \"type\": \"string\"\n    },\n    \"cardHolderInfo\": {\n      \"type\": \"string\"\n    },\n    \"cavvAlgorithm\": {\n      \"type\": \"string\"\n    },\n    \"challengeIndicator\": {\n      \"type\": \"string\"\
  \n    },\n    \"dsReferenceNumber\": {\n      \"type\": \"string\"\n    },\n    \"dsTransID\": {\n      \"type\": \"string\"\n    },\n    \"exemptionIndicator\": {\n      \"type\": \"string\"\n    },\n    \"messageVersion\": {\n      \"type\": \"string\"\n    },\n    \"riskScore\": {\n      \"type\": \"string\"\n    },\n    \"sdkEphemPubKey\": {\n      \"type\": \"string\"\n    },\n    \"threeDSServerTransID\": {\n      \"type\": \"string\"\n    },\n    \"transStatus\": {\n      \"type\": \"string\"\n    },\n    \"transStatusReason\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-three-ds2-response-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDS2ResponseData
---
