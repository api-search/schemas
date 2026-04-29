---
description: AdditionalData3DSecure schema from Adyen API
layout: schema
name: AdditionalData3DSecure
properties_list:
- description: Indicates if you are able to process 3D Secure 2 transactions natively on your payment page. Send this parameter when you are using `/payments` endpoint with any of our [native 3D Secure 2 solutions](
  name: allow3DS2
  type: string
- description: 'Dimensions of the 3DS2 challenge window to be displayed to the cardholder. Possible values: * **01** - size of 250x400 * **02** - size of 390x400 * **03** - size of 500x600 * **04** - size of 600x400 '
  name: challengeWindowSize
  type: string
- description: Indicates if you want to perform 3D Secure authentication on a transaction. > Alternatively, you can use [Dynamic 3D Secure](/risk-management/dynamic-3d-secure) to configure rules for applying 3D Secu
  name: executeThreeD
  type: string
- description: In case of Secure+, this field must be set to **CUPSecurePlus**.
  name: mpiImplementationType
  type: string
- description: Indicates the [exemption type](https://docs.adyen.com/payments-fundamentals/psd2-sca-compliance-and-implementation-guide#specifypreferenceinyourapirequest) that you want to request for the transaction
  name: scaExemption
  type: string
- description: Indicates your preference for the 3D Secure version. > If you use this parameter, you override the checks from Adyen's Authentication Engine. We recommend to use this field only if you have an extensi
  name: threeDSVersion
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-additional-data3-d-secure-schema.json
slug: payments-additional-data3-d-secure
source_filename: payments-additional-data3-d-secure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-additional-data3-d-secure-schema.json\",\n  \"title\": \"AdditionalData3DSecure\",\n  \"description\": \"AdditionalData3DSecure schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allow3DS2\": {\n      \"description\": \"Indicates if you are able to process 3D Secure 2 transactions natively on your payment page. Send this parameter when you are using `/payments` endpoint with any of our [native 3D Secure 2 solutions](https://docs.adyen.com/online-payments/3d-secure/native-3ds2).\\n\\n > This parameter only indicates readiness to support native 3D Secure 2 authentication. To specify if you _want_ to perform 3D Secure, use [Dynamic 3D Secure](/risk-management/dynamic-3d-secure)\\nor send the `executeThreeD` parameter.\\nPossible values:\\n* **true** - Ready to support native 3D Secure\
  \ 2 authentication. Setting this to true does not mean always applying 3D Secure 2. Adyen still selects the version of 3D Secure based on configuration to optimize authorisation rates and improve the shopper's experience.\\n* **false** \\u2013 Not ready to support native 3D Secure 2 authentication. Adyen will not offer 3D Secure 2 to your shopper regardless of your configuration.\\n\",\n      \"type\": \"string\"\n    },\n    \"challengeWindowSize\": {\n      \"description\": \"Dimensions of the 3DS2 challenge window to be displayed to the cardholder.\\n\\nPossible values:\\n\\n* **01** - size of 250x400 \\n* **02** - size of 390x400\\n* **03** - size of 500x600\\n* **04** - size of 600x400\\n* **05** - Fullscreen\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\"\n      ],\n      \"type\": \"string\"\n    },\n    \"executeThreeD\": {\n      \"description\": \"Indicates if you want to perform 3D Secure authentication on a transaction.\\\
  n\\n > Alternatively, you can use [Dynamic 3D Secure](/risk-management/dynamic-3d-secure) to configure rules for applying 3D Secure.\\n\\nPossible values:\\n* **true** \\u2013 Perform 3D Secure authentication.\\n* **false** \\u2013 Don't perform 3D Secure authentication. Note that this setting results in refusals if the issuer mandates 3D Secure because of the PSD2 directive  or other, national regulations. \\n\",\n      \"type\": \"string\"\n    },\n    \"mpiImplementationType\": {\n      \"description\": \"In case of Secure+, this field must be set to **CUPSecurePlus**.\",\n      \"type\": \"string\"\n    },\n    \"scaExemption\": {\n      \"description\": \"Indicates the [exemption type](https://docs.adyen.com/payments-fundamentals/psd2-sca-compliance-and-implementation-guide#specifypreferenceinyourapirequest) that you want to request for the transaction.\\n\\n Possible values:\\n* **lowValue** \\n* **secureCorporate** \\n* **trustedBeneficiary** \\n* **transactionRiskAnalysis** \"\
  ,\n      \"type\": \"string\"\n    },\n    \"threeDSVersion\": {\n      \"description\": \"Indicates your preference for the 3D Secure version. \\n> If you use this parameter, you override the checks from Adyen's Authentication Engine. We recommend to use this field only if you have an extensive knowledge of 3D Secure.\\n\\nPossible values:\\n* **1.0.2**: Apply 3D Secure version 1.0.2. \\n* **2.1.0**: Apply 3D Secure version 2.1.0. \\n* **2.2.0**: Apply 3D Secure version 2.2.0. If the issuer does not support version 2.2.0, we will fall back to 2.1.0.\\n\\nThe following rules apply:\\n* If you prefer 2.1.0 or 2.2.0 but we receive a negative `transStatus` in the `ARes`, we will apply the fallback policy configured in your account. For example, if the configuration is to fall back to 3D Secure 1, we will apply version 1.0.2.\\n* If you prefer 2.1.0 or 2.2.0 but the BIN is not enrolled, you will receive an error.\\n\\n\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-additional-data3-d-secure-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalData3DSecure
---
