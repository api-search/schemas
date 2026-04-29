---
description: AuthenticationInfo schema from Adyen API
layout: schema
name: AuthenticationInfo
properties_list:
- description: Universally unique transaction identifier assigned by the Access Control Server (ACS) to identify a single transaction.
  name: acsTransId
  type: string
- description: Information about Strong Customer Authentication (SCA). Returned when `type` is **challenge**.
  name: challenge
  type: object
- description: 'Specifies a preference for receiving a challenge. Possible values: * **01**: No preference * **02**: No challenge requested * **03**: Challenge requested (preference) * **04**: Challenge requested (ma'
  name: challengeIndicator
  type: string
- description: 'Date and time in UTC of the cardholder authentication. [ISO 8601](https://www.w3.org/TR/NOTE-datetime) format: YYYY-MM-DDThh:mm:ss+TZD, for example, **2020-12-18T10:15:30+01:00**.'
  name: createdAt
  type: string
- description: 'Indicates the type of channel interface being used to initiate the transaction. Possible values: * **app** * **browser** * **3DSRequestorInitiated** (initiated by a merchant when the cardholder is not'
  name: deviceChannel
  type: string
- description: Universally unique transaction identifier assigned by the DS (card scheme) to identify a single transaction.
  name: dsTransID
  type: string
- description: 'Indicates the exemption type that was applied to the authentication by the issuer, if exemption applied. Possible values: * **lowValue** * **secureCorporate** * **trustedBeneficiary** * **transactionR'
  name: exemptionIndicator
  type: string
- description: Indicates if the purchase was in the PSD2 scope.
  name: inPSD2Scope
  type: boolean
- description: 'Identifies the category of the message for a specific use case. Possible values: * **payment** * **nonPayment**'
  name: messageCategory
  type: string
- description: The `messageVersion` value as defined in the 3D Secure 2 specification.
  name: messageVersion
  type: string
- description: Risk score calculated from the transaction rules.
  name: riskScore
  type: integer
- description: The `threeDSServerTransID` value as defined in the 3D Secure 2 specification.
  name: threeDSServerTransID
  type: string
- description: 'The `transStatus` value as defined in the 3D Secure 2 specification. Possible values: * **Y**: Authentication / Account verification successful. * **N**: Not Authenticated / Account not verified. Tran'
  name: transStatus
  type: string
- description: Provides information on why the `transStatus` field has the specified value. For possible values, refer to [our docs](https://docs.adyen.com/online-payments/3d-secure/api-reference#possible-transstatu
  name: transStatusReason
  type: string
- description: 'The type of authentication performed. Possible values: * **frictionless** * **challenge**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/authentication-webhooks-authentication-info-schema.json
slug: authentication-webhooks-authentication-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/authentication-webhooks-authentication-info-schema.json\",\n  \"title\": \"AuthenticationInfo\",\n  \"description\": \"AuthenticationInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acsTransId\": {\n      \"description\": \"Universally unique transaction identifier assigned by the Access Control Server (ACS) to identify a single transaction.\",\n      \"type\": \"string\"\n    },\n    \"challenge\": {\n      \"description\": \"Information about Strong Customer Authentication (SCA). Returned when `type` is **challenge**.\",\n      \"$ref\": \"#/components/schemas/ChallengeInfo\"\n    },\n    \"challengeIndicator\": {\n      \"description\": \"Specifies a preference for receiving a challenge. Possible values:\\n\\n* **01**: No preference\\n* **02**: No challenge requested\\n* **03**:\
  \ Challenge requested (preference)\\n* **04**: Challenge requested (mandate)\\n* **05**: No challenge requested (transactional risk analysis is already performed)\\n* **07**: No challenge requested (SCA is already performed)\\n* **08**: No challenge requested (trusted beneficiaries exemption of no challenge required)\\n* **09**: Challenge requested (trusted beneficiaries prompt requested if challenge required)\\n* **80**: No challenge requested (secure corporate payment with Mastercard)\\n* **82**: No challenge requested (secure corporate payment with Visa)\\n\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\",\n        \"07\",\n        8,\n        9,\n        \"80\",\n        \"82\"\n      ],\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"description\": \"Date and time in UTC of the cardholder authentication. \\n\\n[ISO 8601](https://www.w3.org/TR/NOTE-datetime) format: YYYY-MM-DDThh:mm:ss+TZD, for example, **2020-12-18T10:15:30+01:00**.\"\
  ,\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"deviceChannel\": {\n      \"description\": \"Indicates the type of channel interface being used to initiate the transaction. Possible values:\\n\\n* **app**\\n* **browser**\\n* **3DSRequestorInitiated** (initiated by a merchant when the cardholder is not available)\",\n      \"enum\": [\n        \"app\",\n        \"browser\",\n        \"ThreeDSRequestorInitiated\"\n      ],\n      \"type\": \"string\"\n    },\n    \"dsTransID\": {\n      \"description\": \"Universally unique transaction identifier assigned by the DS (card scheme) to identify a single transaction.\",\n      \"type\": \"string\"\n    },\n    \"exemptionIndicator\": {\n      \"description\": \"Indicates the exemption type that was applied to the authentication by the issuer, if exemption applied. Possible values:\\n\\n* **lowValue**\\n* **secureCorporate**\\n* **trustedBeneficiary**\\n* **transactionRiskAnalysis**\\n* **acquirerExemption**\\n*\
  \ **noExemptionApplied**\\n* **visaDAFExemption**\\n\",\n      \"enum\": [\n        \"lowValue\",\n        \"secureCorporate\",\n        \"trustedBeneficiary\",\n        \"transactionRiskAnalysis\",\n        \"acquirerExemption\",\n        \"noExemptionApplied\",\n        \"visaDAFExemption\"\n      ],\n      \"type\": \"string\"\n    },\n    \"inPSD2Scope\": {\n      \"description\": \"Indicates if the purchase was in the PSD2 scope.\",\n      \"type\": \"boolean\"\n    },\n    \"messageCategory\": {\n      \"description\": \"Identifies the category of the message for a specific use case. Possible values:\\n\\n* **payment**\\n* **nonPayment**\",\n      \"enum\": [\n        \"payment\",\n        \"nonPayment\"\n      ],\n      \"type\": \"string\"\n    },\n    \"messageVersion\": {\n      \"description\": \"The `messageVersion` value as defined in the 3D Secure 2 specification.\",\n      \"type\": \"string\"\n    },\n    \"riskScore\": {\n      \"description\": \"Risk score calculated\
  \ from the transaction rules.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"threeDSServerTransID\": {\n      \"description\": \"The `threeDSServerTransID` value as defined in the 3D Secure 2 specification.\",\n      \"type\": \"string\"\n    },\n    \"transStatus\": {\n      \"description\": \"The `transStatus` value as defined in the 3D Secure 2 specification. Possible values:\\n\\n* **Y**: Authentication / Account verification successful.\\n* **N**: Not Authenticated / Account not verified. Transaction denied.\\n* **U**: Authentication / Account verification could not be performed.\\n* **I**: Informational Only / 3D Secure Requestor challenge preference acknowledged.\\n* **R**: Authentication / Account verification rejected by the Issuer.\\n\",\n      \"enum\": [\n        \"Y\",\n        \"N\",\n        \"R\",\n        \"I\",\n        \"U\"\n      ],\n      \"type\": \"string\"\n    },\n    \"transStatusReason\": {\n      \"description\": \"Provides information\
  \ on why the `transStatus` field has the specified value. For possible values, refer to [our docs](https://docs.adyen.com/online-payments/3d-secure/api-reference#possible-transstatusreason-values).\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\",\n        \"06\",\n        \"07\",\n        8,\n        9,\n        \"10\",\n        \"11\",\n        \"12\",\n        \"13\",\n        \"14\",\n        \"15\",\n        \"16\",\n        \"17\",\n        \"18\",\n        \"19\",\n        \"20\",\n        \"21\",\n        \"22\",\n        \"23\",\n        \"24\",\n        \"25\",\n        \"26\",\n        \"80\",\n        \"81\",\n        \"82\",\n        \"83\",\n        \"84\",\n        \"85\",\n        \"86\",\n        \"87\",\n        \"88\"\n      ],\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of authentication performed. Possible values:\\n\\n* **frictionless**\\n* **challenge**\",\n     \
  \ \"enum\": [\n        \"frictionless\",\n        \"challenge\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"challengeIndicator\",\n    \"dsTransID\",\n    \"messageVersion\",\n    \"threeDSServerTransID\",\n    \"transStatus\",\n    \"createdAt\",\n    \"type\",\n    \"inPSD2Scope\",\n    \"deviceChannel\",\n    \"messageCategory\",\n    \"acsTransId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/authentication-webhooks-authentication-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AuthenticationInfo
---
