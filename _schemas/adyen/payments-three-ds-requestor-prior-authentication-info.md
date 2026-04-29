---
description: ThreeDSRequestorPriorAuthenticationInfo schema from Adyen API
layout: schema
name: ThreeDSRequestorPriorAuthenticationInfo
properties_list:
- description: 'Data that documents and supports a specific authentication process. Maximum length: 2048 bytes.'
  name: threeDSReqPriorAuthData
  type: string
- description: 'Mechanism used by the Cardholder to previously authenticate to the 3DS Requestor. Allowed values: * **01** — Frictionless authentication occurred by ACS. * **02** — Cardholder challenge occurred by AC'
  name: threeDSReqPriorAuthMethod
  type: string
- description: 'Date and time in UTC of the prior cardholder authentication. Format: YYYYMMDDHHMM'
  name: threeDSReqPriorAuthTimestamp
  type: string
- description: This data element provides additional information to the ACS to determine the best approach for handing a request. This data element contains an ACS Transaction ID for a prior authenticated transactio
  name: threeDSReqPriorRef
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-three-ds-requestor-prior-authentication-info-schema.json
slug: payments-three-ds-requestor-prior-authentication-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-three-ds-requestor-prior-authentication-info-schema.json\",\n  \"title\": \"ThreeDSRequestorPriorAuthenticationInfo\",\n  \"description\": \"ThreeDSRequestorPriorAuthenticationInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"threeDSReqPriorAuthData\": {\n      \"description\": \"Data that documents and supports a specific authentication process. Maximum length: 2048 bytes.\",\n      \"type\": \"string\"\n    },\n    \"threeDSReqPriorAuthMethod\": {\n      \"description\": \"Mechanism used by the Cardholder to previously authenticate to the 3DS Requestor. Allowed values:\\n* **01** \\u2014 Frictionless authentication occurred by ACS.\\n* **02** \\u2014 Cardholder challenge occurred by ACS.\\n* **03** \\u2014 AVS verified.\\n* **04** \\u2014 Other issuer methods.\",\n   \
  \   \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\"\n      ],\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"threeDSReqPriorAuthTimestamp\": {\n      \"description\": \"Date and time in UTC of the prior cardholder authentication. Format: YYYYMMDDHHMM\",\n      \"maxLength\": 12,\n      \"minLength\": 12,\n      \"type\": \"string\"\n    },\n    \"threeDSReqPriorRef\": {\n      \"description\": \"This data element provides additional information to the ACS to determine the best approach for handing a request. This data element contains an ACS Transaction ID for a prior authenticated transaction. For example, the first recurring transaction that was authenticated with the cardholder. Length: 30 characters.\",\n      \"maxLength\": 36,\n      \"minLength\": 36,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-three-ds-requestor-prior-authentication-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDSRequestorPriorAuthenticationInfo
---
