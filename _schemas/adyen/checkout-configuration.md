---
description: Configuration schema from Adyen API
layout: schema
name: Configuration
properties_list:
- description: Describes the configuration for AVS ([Address Verification System](https://en.wikipedia.org/wiki/Address_Verification_System)).
  name: avs
  type: object
- description: 'Determines whether the cardholder name should be provided or not. Permitted values: * NONE * OPTIONAL * REQUIRED'
  name: cardHolderName
  type: string
- description: Describes the configuration for [installment payments](https://docs.adyen.com/payment-methods/cards/credit-card-installments).
  name: installments
  type: object
- description: Determines how to display the details fields.
  name: shopperInput
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-configuration-schema.json
slug: checkout-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-configuration-schema.json\",\n  \"title\": \"Configuration\",\n  \"description\": \"Configuration schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"avs\": {\n      \"description\": \"Describes the configuration for AVS ([Address Verification System](https://en.wikipedia.org/wiki/Address_Verification_System)).\",\n      \"$ref\": \"#/components/schemas/Avs\"\n    },\n    \"cardHolderName\": {\n      \"x-addedInVersion\": \"37\",\n      \"description\": \"Determines whether the cardholder name should be provided or not.\\n\\nPermitted values:\\n* NONE\\n* OPTIONAL\\n* REQUIRED\",\n      \"enum\": [\n        \"NONE\",\n        \"OPTIONAL\",\n        \"REQUIRED\"\n      ],\n      \"type\": \"string\"\n    },\n    \"installments\": {\n      \"description\": \"Describes the configuration\
  \ for [installment payments](https://docs.adyen.com/payment-methods/cards/credit-card-installments).\",\n      \"$ref\": \"#/components/schemas/InstallmentsNumber\"\n    },\n    \"shopperInput\": {\n      \"x-addedInVersion\": \"37\",\n      \"description\": \"Determines how to display the details fields.\",\n      \"$ref\": \"#/components/schemas/ShopperInput\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-configuration-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Configuration
---
