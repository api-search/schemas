---
description: ThreeDSRequestData schema from Adyen API
layout: schema
name: ThreeDSRequestData
properties_list:
- description: 'Dimensions of the 3DS2 challenge window to be displayed to the cardholder. Possible values: * **01** - size of 250x400 * **02** - size of 390x400 * **03** - size of 500x600 * **04** - size of 600x400 '
  name: challengeWindowSize
  type: string
- description: Flag for data only flow.
  name: dataOnly
  type: string
- description: 'Indicates if [native 3D Secure authentication](https://docs.adyen.com/online-payments/3d-secure/native-3ds2) should be used when available. Possible values: * **preferred**: Use native 3D Secure authe'
  name: nativeThreeDS
  type: string
- description: 'The version of 3D Secure to use. Possible values: * **2.1.0** * **2.2.0**'
  name: threeDSVersion
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-three-ds-request-data-schema.json
slug: checkout-three-ds-request-data
source_filename: checkout-three-ds-request-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-three-ds-request-data-schema.json\",\n  \"title\": \"ThreeDSRequestData\",\n  \"description\": \"ThreeDSRequestData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"challengeWindowSize\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"Dimensions of the 3DS2 challenge window to be displayed to the cardholder.\\n\\nPossible values:\\n\\n* **01** - size of 250x400 \\n* **02** - size of 390x400\\n* **03** - size of 500x600\\n* **04** - size of 600x400\\n* **05** - Fullscreen\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\"\n      ],\n      \"type\": \"string\"\n    },\n    \"dataOnly\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"Flag for data only flow.\",\n      \"enum\": [\n      \
  \  \"false\",\n        \"true\"\n      ],\n      \"type\": \"string\"\n    },\n    \"nativeThreeDS\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"Indicates if [native 3D Secure authentication](https://docs.adyen.com/online-payments/3d-secure/native-3ds2) should be used when available.\\n\\nPossible values:\\n* **preferred**: Use native 3D Secure authentication when available.\",\n      \"enum\": [\n        \"preferred\"\n      ],\n      \"type\": \"string\"\n    },\n    \"threeDSVersion\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"The version of 3D Secure to use.\\n\\nPossible values:\\n\\n* **2.1.0**\\n* **2.2.0**\",\n      \"enum\": [\n        \"2.1.0\",\n        \"2.2.0\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-three-ds-request-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ThreeDSRequestData
---
