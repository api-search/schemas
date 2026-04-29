---
description: ResponseAdditionalData3DSecure schema from Adyen API
layout: schema
name: ResponseAdditionalData3DSecure
properties_list:
- description: Information provided by the issuer to the cardholder. If this field is present, you need to display this information to the cardholder.
  name: cardHolderInfo
  type: string
- description: The Cardholder Authentication Verification Value (CAVV) for the 3D Secure authentication session, as a Base64-encoded 20-byte array.
  name: cavv
  type: string
- description: The CAVV algorithm used.
  name: cavvAlgorithm
  type: string
- description: Shows the [exemption type](https://docs.adyen.com/payments-fundamentals/psd2-sca-compliance-and-implementation-guide#specifypreferenceinyourapirequest) that Adyen requested for the payment. Possible v
  name: scaExemptionRequested
  type: string
- description: Indicates whether a card is enrolled for 3D Secure 2.
  name: threeds2.cardEnrolled
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payouts-response-additional-data3-d-secure-schema.json
slug: payouts-response-additional-data3-d-secure
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-response-additional-data3-d-secure-schema.json\",\n  \"title\": \"ResponseAdditionalData3DSecure\",\n  \"description\": \"ResponseAdditionalData3DSecure schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardHolderInfo\": {\n      \"description\": \"Information provided by the issuer to the cardholder. If this field is present, you need to display this information to the cardholder. \",\n      \"type\": \"string\"\n    },\n    \"cavv\": {\n      \"description\": \"The Cardholder Authentication Verification Value (CAVV) for the 3D Secure authentication session, as a Base64-encoded 20-byte array.\",\n      \"type\": \"string\"\n    },\n    \"cavvAlgorithm\": {\n      \"description\": \"The CAVV algorithm used.\",\n      \"type\": \"string\"\n    },\n    \"scaExemptionRequested\"\
  : {\n      \"description\": \"Shows the [exemption type](https://docs.adyen.com/payments-fundamentals/psd2-sca-compliance-and-implementation-guide#specifypreferenceinyourapirequest) that Adyen requested for the payment.\\n\\n Possible values:\\n* **lowValue** \\n* **secureCorporate** \\n* **trustedBeneficiary** \\n* **transactionRiskAnalysis** \",\n      \"type\": \"string\"\n    },\n    \"threeds2.cardEnrolled\": {\n      \"description\": \"Indicates whether a card is enrolled for 3D Secure 2.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-response-additional-data3-d-secure-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ResponseAdditionalData3DSecure
---
