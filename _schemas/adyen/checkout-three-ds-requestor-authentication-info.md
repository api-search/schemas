---
description: ThreeDSRequestorAuthenticationInfo schema from Adyen API
layout: schema
name: ThreeDSRequestorAuthenticationInfo
properties_list:
- description: 'Data that documents and supports a specific authentication process. Maximum length: 2048 bytes.'
  name: threeDSReqAuthData
  type: string
- description: 'Mechanism used by the Cardholder to authenticate to the 3DS Requestor. Allowed values: * **01** — No 3DS Requestor authentication occurred (for example, cardholder “logged in” as guest). * **02** — Lo'
  name: threeDSReqAuthMethod
  type: string
- description: 'Date and time in UTC of the cardholder authentication. Format: YYYYMMDDHHMM'
  name: threeDSReqAuthTimestamp
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-three-ds-requestor-authentication-info-schema.json
slug: checkout-three-ds-requestor-authentication-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-three-ds-requestor-authentication-info-schema.json\",\n  \"title\": \"ThreeDSRequestorAuthenticationInfo\",\n  \"description\": \"ThreeDSRequestorAuthenticationInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"threeDSReqAuthData\": {\n      \"description\": \"Data that documents and supports a specific authentication process. Maximum length: 2048 bytes.\",\n      \"type\": \"string\"\n    },\n    \"threeDSReqAuthMethod\": {\n      \"description\": \"Mechanism used by the Cardholder to authenticate to the 3DS Requestor. Allowed values:\\n* **01** \\u2014 No 3DS Requestor authentication occurred (for example, cardholder \\u201clogged in\\u201d as guest).\\n* **02** \\u2014 Login to the cardholder account at the 3DS Requestor system using 3DS Requestor\\u2019s own credentials.\\\
  n* **03** \\u2014 Login to the cardholder account at the 3DS Requestor system using federated ID.\\n* **04** \\u2014 Login to the cardholder account at the 3DS Requestor system using issuer credentials.\\n* **05** \\u2014 Login to the cardholder account at the 3DS Requestor system using third-party authentication.\\n* **06** \\u2014 Login to the cardholder account at the 3DS Requestor system using FIDO Authenticator.\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\",\n        \"06\"\n      ],\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"threeDSReqAuthTimestamp\": {\n      \"description\": \"Date and time in UTC of the cardholder authentication. Format: YYYYMMDDHHMM\",\n      \"maxLength\": 12,\n      \"minLength\": 12,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-three-ds-requestor-authentication-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDSRequestorAuthenticationInfo
---
