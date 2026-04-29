---
description: ThreeDS2Result schema from Adyen API
layout: schema
name: ThreeDS2Result
properties_list:
- description: The `authenticationValue` value as defined in the 3D Secure 2 specification.
  name: authenticationValue
  type: string
- description: The algorithm used by the ACS to calculate the authentication value, only for Cartes Bancaires integrations.
  name: cavvAlgorithm
  type: string
- description: Indicator informing the Access Control Server (ACS) and the Directory Server (DS) that the authentication has been cancelled. For possible values, refer to [3D Secure API reference](https://docs.adyen
  name: challengeCancel
  type: string
- description: The `dsTransID` value as defined in the 3D Secure 2 specification.
  name: dsTransID
  type: string
- description: The `eci` value as defined in the 3D Secure 2 specification.
  name: eci
  type: string
- description: 'Indicates the exemption type that was applied by the issuer to the authentication, if exemption applied. Allowed values: * `lowValue` * `secureCorporate` * `trustedBeneficiary` * `transactionRiskAnaly'
  name: exemptionIndicator
  type: string
- description: The `messageVersion` value as defined in the 3D Secure 2 specification.
  name: messageVersion
  type: string
- description: Risk score calculated by Cartes Bancaires Directory Server (DS).
  name: riskScore
  type: string
- description: 'Indicates whether a challenge is requested for this transaction. Possible values: * **01** — No preference * **02** — No challenge requested * **03** — Challenge requested (3DS Requestor preference) *'
  name: threeDSRequestorChallengeInd
  type: string
- description: The `threeDSServerTransID` value as defined in the 3D Secure 2 specification.
  name: threeDSServerTransID
  type: string
- description: The `timestamp` value of the 3D Secure 2 authentication.
  name: timestamp
  type: string
- description: The `transStatus` value as defined in the 3D Secure 2 specification.
  name: transStatus
  type: string
- description: Provides information on why the `transStatus` field has the specified value. For possible values, refer to [our docs](https://docs.adyen.com/online-payments/3d-secure/api-reference#possible-transstatu
  name: transStatusReason
  type: string
- description: The `whiteListStatus` value as defined in the 3D Secure 2 specification.
  name: whiteListStatus
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-three-ds2-result-schema.json
slug: checkout-three-ds2-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-three-ds2-result-schema.json\",\n  \"title\": \"ThreeDS2Result\",\n  \"description\": \"ThreeDS2Result schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authenticationValue\": {\n      \"description\": \"The `authenticationValue` value as defined in the 3D Secure 2 specification.\",\n      \"type\": \"string\"\n    },\n    \"cavvAlgorithm\": {\n      \"x-addedInVersion\": \"50\",\n      \"description\": \"The algorithm used by the ACS to calculate the authentication value, only for Cartes Bancaires integrations.\",\n      \"type\": \"string\"\n    },\n    \"challengeCancel\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"Indicator informing the Access Control Server (ACS) and the Directory Server (DS) that the authentication has been cancelled. For possible\
  \ values, refer to [3D Secure API reference](https://docs.adyen.com/online-payments/3d-secure/api-reference#mpidata).\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\",\n        \"06\",\n        \"07\"\n      ],\n      \"type\": \"string\"\n    },\n    \"dsTransID\": {\n      \"description\": \"The `dsTransID` value as defined in the 3D Secure 2 specification.\",\n      \"type\": \"string\"\n    },\n    \"eci\": {\n      \"description\": \"The `eci` value as defined in the 3D Secure 2 specification.\",\n      \"type\": \"string\"\n    },\n    \"exemptionIndicator\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"Indicates the exemption type that was applied by the issuer to the authentication, if exemption applied.\\nAllowed values:\\n* `lowValue`\\n* `secureCorporate`\\n* `trustedBeneficiary`\\n* `transactionRiskAnalysis`\\n\",\n      \"enum\": [\n        \"lowValue\",\n        \"secureCorporate\",\n        \"trustedBeneficiary\"\
  ,\n        \"transactionRiskAnalysis\"\n      ],\n      \"type\": \"string\"\n    },\n    \"messageVersion\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"The `messageVersion` value as defined in the 3D Secure 2 specification.\",\n      \"type\": \"string\"\n    },\n    \"riskScore\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"Risk score calculated by Cartes Bancaires Directory Server (DS).\",\n      \"type\": \"string\"\n    },\n    \"threeDSRequestorChallengeInd\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Indicates whether a challenge is requested for this transaction. Possible values:\\n* **01** \\u2014 No preference\\n* **02** \\u2014 No challenge requested\\n* **03** \\u2014 Challenge requested (3DS Requestor preference)\\n* **04** \\u2014 Challenge requested (Mandate)\\n* **05** \\u2014 No challenge (transactional risk analysis is already performed)\\n* **06** \\u2014 Data Only\",\n      \"enum\": [\n        \"01\"\
  ,\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\",\n        \"06\"\n      ],\n      \"type\": \"string\"\n    },\n    \"threeDSServerTransID\": {\n      \"description\": \"The `threeDSServerTransID` value as defined in the 3D Secure 2 specification.\",\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"description\": \"The `timestamp` value of the 3D Secure 2 authentication.\",\n      \"type\": \"string\"\n    },\n    \"transStatus\": {\n      \"description\": \"The `transStatus` value as defined in the 3D Secure 2 specification.\",\n      \"type\": \"string\"\n    },\n    \"transStatusReason\": {\n      \"description\": \"Provides information on why the `transStatus` field has the specified value. For possible values, refer to [our docs](https://docs.adyen.com/online-payments/3d-secure/api-reference#possible-transstatusreason-values).\",\n      \"type\": \"string\"\n    },\n    \"whiteListStatus\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\"\
  : \"The `whiteListStatus` value as defined in the 3D Secure 2 specification.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-three-ds2-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDS2Result
---
