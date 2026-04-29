---
description: UpdateStoreRequest schema from Adyen API
layout: schema
name: UpdateStoreRequest
properties_list:
- description: The address of the store. It is not possible to update the country of the store.
  name: address
  type: object
- description: The unique identifiers of the [business lines](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/businessLines__resParam_id) that the store is associated with.
  name: businessLineIds
  type: array
- description: The description of the store.
  name: description
  type: string
- description: The unique identifier of the store, used by certain payment methods and tax authorities. Accepts up to 14 digits. Required for CNPJ in Brazil, in the format 00.000.000/00git00-00 separated by dots, sl
  name: externalReferenceId
  type: string
- description: The phone number of the store, including '+' and country code in the [E.164](https://en.wikipedia.org/wiki/E.164) format. If passed in a different format, we convert and validate the phone number agai
  name: phoneNumber
  type: string
- description: Rules for Adyen for Platforms merchants to split the transaction amount and fees.
  name: splitConfiguration
  type: object
- description: 'The status of the store. Possible values are: - **active**: This value is assigned automatically when a store is created. - **inactive**: The maximum [transaction limits and number of Store-and-Forwar'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-update-store-request-schema.json
slug: management-update-store-request
source_filename: management-update-store-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-store-request-schema.json\",\n  \"title\": \"UpdateStoreRequest\",\n  \"description\": \"UpdateStoreRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address of the store. It is not possible to update the country of the store.\",\n      \"$ref\": \"#/components/schemas/UpdatableAddress\"\n    },\n    \"businessLineIds\": {\n      \"description\": \"The unique identifiers of the [business lines](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/businessLines__resParam_id) that the store is associated with.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"description\": {\n      \"description\": \"The description of the store.\",\n      \"type\": \"string\"\
  \n    },\n    \"externalReferenceId\": {\n      \"description\": \"The unique identifier of the store, used by certain payment methods and tax authorities. Accepts up to 14 digits.\\n\\nRequired for CNPJ in Brazil, in the format 00.000.000/00git00-00 separated by dots, slashes, hyphens, or without separators.\\n\\nOptional for Zip in Australia and SIRET in France, required except for nonprofit organizations and incorporated associations.\\n\\n\",\n      \"type\": \"string\"\n    },\n    \"phoneNumber\": {\n      \"description\": \"The phone number of the store, including '+' and country code in the [E.164](https://en.wikipedia.org/wiki/E.164) format. If passed in a different format, we convert and validate the phone number against E.164. \",\n      \"type\": \"string\"\n    },\n    \"splitConfiguration\": {\n      \"description\": \"Rules for Adyen for Platforms merchants to split the transaction amount and fees.\",\n      \"$ref\": \"#/components/schemas/StoreSplitConfiguration\"\n  \
  \  },\n    \"status\": {\n      \"description\": \"The status of the store. Possible values are:\\n\\n- **active**: This value is assigned automatically when a store is created. \\n- **inactive**: The maximum [transaction limits and number of Store-and-Forward transactions](https://docs.adyen.com/point-of-sale/determine-account-structure/configure-features#payment-features) for the store are set to 0. This blocks new transactions, but captures are still possible.\\n- **closed**: The terminals of the store are reassigned to the merchant inventory, so they can't process payments.\\n\\nYou can change the status from **active** to **inactive**, and from **inactive** to **active** or **closed**. \\nOnce **closed**, a store can't be reopened.\",\n      \"enum\": [\n        \"active\",\n        \"closed\",\n        \"inactive\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-update-store-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdateStoreRequest
---
