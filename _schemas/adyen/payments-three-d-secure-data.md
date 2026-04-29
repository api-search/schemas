---
description: ThreeDSecureData schema from Adyen API
layout: schema
name: ThreeDSecureData
properties_list:
- description: In 3D Secure 1, the authentication response if the shopper was redirected. In 3D Secure 2, this is the `transStatus` from the challenge result. If the transaction was frictionless, omit this parameter
  name: authenticationResponse
  type: string
- description: The cardholder authentication value (base64 encoded, 20 bytes in a decoded form).
  name: cavv
  type: string
- description: The CAVV algorithm used. Include this only for 3D Secure 1.
  name: cavvAlgorithm
  type: string
- description: Indicator informing the Access Control Server (ACS) and the Directory Server (DS) that the authentication has been cancelled. For possible values, refer to [3D Secure API reference](https://docs.adyen
  name: challengeCancel
  type: string
- description: In 3D Secure 1, this is the enrollment response from the 3D directory server. In 3D Secure 2, this is the `transStatus` from the `ARes`.
  name: directoryResponse
  type: string
- description: Supported for 3D Secure 2. The unique transaction identifier assigned by the Directory Server (DS) to identify a single transaction.
  name: dsTransID
  type: string
- description: The electronic commerce indicator.
  name: eci
  type: string
- description: Risk score calculated by Directory Server (DS). Required for Cartes Bancaires integrations.
  name: riskScore
  type: string
- description: The version of the 3D Secure protocol.
  name: threeDSVersion
  type: string
- description: Network token authentication verification value (TAVV). The network token cryptogram.
  name: tokenAuthenticationVerificationValue
  type: string
- description: Provides information on why the `transStatus` field has the specified value. For possible values, refer to [our docs](https://docs.adyen.com/online-payments/3d-secure/api-reference#possible-transstatu
  name: transStatusReason
  type: string
- description: Supported for 3D Secure 1. The transaction identifier (Base64-encoded, 20 bytes in a decoded form).
  name: xid
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-three-d-secure-data-schema.json
slug: payments-three-d-secure-data
source_filename: payments-three-d-secure-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-three-d-secure-data-schema.json\",\n  \"title\": \"ThreeDSecureData\",\n  \"description\": \"ThreeDSecureData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authenticationResponse\": {\n      \"description\": \"In 3D Secure 1, the authentication response if the shopper was redirected.\\n\\nIn 3D Secure 2, this is the `transStatus` from the challenge result. If the transaction was frictionless, omit this parameter.\",\n      \"enum\": [\n        \"Y\",\n        \"N\",\n        \"U\",\n        \"A\"\n      ],\n      \"type\": \"string\"\n    },\n    \"cavv\": {\n      \"description\": \"The cardholder authentication value (base64 encoded, 20 bytes in a decoded form).\",\n      \"format\": \"byte\",\n      \"type\": \"string\"\n    },\n    \"cavvAlgorithm\": {\n      \"description\"\
  : \"The CAVV algorithm used. Include this only for 3D Secure 1.\",\n      \"type\": \"string\"\n    },\n    \"challengeCancel\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"Indicator informing the Access Control Server (ACS) and the Directory Server (DS) that the authentication has been cancelled. For possible values, refer to [3D Secure API reference](https://docs.adyen.com/online-payments/3d-secure/api-reference#mpidata).\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\",\n        \"06\",\n        \"07\"\n      ],\n      \"type\": \"string\"\n    },\n    \"directoryResponse\": {\n      \"description\": \"In 3D Secure 1, this is the enrollment response from the 3D directory server.\\n\\nIn 3D Secure 2, this is the `transStatus` from the `ARes`.\",\n      \"enum\": [\n        \"A\",\n        \"C\",\n        \"D\",\n        \"I\",\n        \"N\",\n        \"R\",\n        \"U\",\n        \"Y\"\n      ],\n      \"\
  type\": \"string\"\n    },\n    \"dsTransID\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"Supported for 3D Secure 2. The unique transaction identifier assigned by the Directory Server (DS) to identify a single transaction.\",\n      \"type\": \"string\"\n    },\n    \"eci\": {\n      \"description\": \"The electronic commerce indicator.\",\n      \"type\": \"string\"\n    },\n    \"riskScore\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"Risk score calculated by Directory Server (DS). Required for Cartes Bancaires integrations.\",\n      \"type\": \"string\"\n    },\n    \"threeDSVersion\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"The version of the 3D Secure protocol.\",\n      \"type\": \"string\"\n    },\n    \"tokenAuthenticationVerificationValue\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Network token authentication verification value (TAVV). The network token cryptogram.\",\n      \"format\"\
  : \"byte\",\n      \"type\": \"string\"\n    },\n    \"transStatusReason\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"Provides information on why the `transStatus` field has the specified value. For possible values, refer to [our docs](https://docs.adyen.com/online-payments/3d-secure/api-reference#possible-transstatusreason-values).\",\n      \"type\": \"string\"\n    },\n    \"xid\": {\n      \"description\": \"Supported for 3D Secure 1. The transaction identifier (Base64-encoded, 20 bytes in a decoded form).\",\n      \"format\": \"byte\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-three-d-secure-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDSecureData
---
