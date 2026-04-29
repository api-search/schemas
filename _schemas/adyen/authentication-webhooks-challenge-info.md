---
description: ChallengeInfo schema from Adyen API
layout: schema
name: ChallengeInfo
properties_list:
- description: Indicator informing the Access Control Server (ACS) and the Directory Server (DS) that the authentication has been cancelled. For possible values, refer to [3D Secure API reference](https://docs.adyen
  name: challengeCancel
  type: string
- description: 'The flow used in the challenge. Possible values: * **OTP_SMS**: one-time password (OTP) flow * **OOB**: out-of-band (OOB) flow'
  name: flow
  type: string
- description: The last time of interaction with the challenge.
  name: lastInteraction
  type: string
- description: The last four digits of the phone number used in the challenge.
  name: phoneNumber
  type: string
- description: The number of times the one-time password (OTP) was resent during the challenge.
  name: resends
  type: integer
- description: The number of retries used in the challenge.
  name: retries
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/authentication-webhooks-challenge-info-schema.json
slug: authentication-webhooks-challenge-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/authentication-webhooks-challenge-info-schema.json\",\n  \"title\": \"ChallengeInfo\",\n  \"description\": \"ChallengeInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"challengeCancel\": {\n      \"description\": \"Indicator informing the Access Control Server (ACS) and the Directory Server (DS) that the authentication has been cancelled. For possible values, refer to [3D Secure API reference](https://docs.adyen.com/online-payments/3d-secure/api-reference#mpidata).\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\",\n        \"06\",\n        \"07\"\n      ],\n      \"type\": \"string\"\n    },\n    \"flow\": {\n      \"description\": \"The flow used in the challenge. Possible values:\\n\\n* **OTP_SMS**: one-time password (OTP)\
  \ flow\\n* **OOB**: out-of-band (OOB) flow\",\n      \"enum\": [\n        \"OTP_SMS\",\n        \"OOB\"\n      ],\n      \"type\": \"string\"\n    },\n    \"lastInteraction\": {\n      \"description\": \"The last time of interaction with the challenge.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"phoneNumber\": {\n      \"description\": \"The last four digits of the phone number used in the challenge.\",\n      \"type\": \"string\"\n    },\n    \"resends\": {\n      \"description\": \"The number of times the one-time password (OTP) was resent during the challenge.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"retries\": {\n      \"description\": \"The number of retries used in the challenge.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"flow\",\n    \"lastInteraction\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/authentication-webhooks-challenge-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ChallengeInfo
---
