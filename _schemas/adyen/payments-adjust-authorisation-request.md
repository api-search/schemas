---
description: AdjustAuthorisationRequest schema from Adyen API
layout: schema
name: AdjustAuthorisationRequest
properties_list:
- description: This field contains additional data, which may be required for a particular modification request. The additionalData object consists of entries, each of which includes the key and value.
  name: additionalData
  type: object
- description: The merchant account that is used to process the payment.
  name: merchantAccount
  type: string
- description: The amount that needs to be adjusted. The `currency` must match the currency used in authorisation, the `value` must be smaller than or equal to the authorised amount.
  name: modificationAmount
  type: object
- description: Authentication data produced by an MPI (Mastercard SecureCode, Visa Secure, or Cartes Bancaires).
  name: mpiData
  type: object
- description: The original merchant reference to cancel.
  name: originalMerchantReference
  type: string
- description: 'The original pspReference of the payment to modify. This reference is returned in: * authorisation response * authorisation notification'
  name: originalReference
  type: string
- description: Defines how to book chargebacks when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#chargebacks-and-disputes).
  name: platformChargebackLogic
  type: object
- description: 'Your reference for the payment modification. This reference is visible in Customer Area and in reports. Maximum length: 80 characters.'
  name: reference
  type: string
- description: An array of objects specifying how the amount should be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-a
  name: splits
  type: array
- description: The transaction reference provided by the PED. For point-of-sale integrations only.
  name: tenderReference
  type: string
- description: Unique terminal ID for the PED that originally processed the request. For point-of-sale integrations only.
  name: uniqueTerminalId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-adjust-authorisation-request-schema.json
slug: payments-adjust-authorisation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-adjust-authorisation-request-schema.json\",\n  \"title\": \"AdjustAuthorisationRequest\",\n  \"description\": \"AdjustAuthorisationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"x-anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdditionalData3DSecure\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataAirline\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataCarRental\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataCommon\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataLevel23\"\n        },\n        {\n          \"\
  $ref\": \"#/components/schemas/AdditionalDataLodging\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataModifications\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataOpenInvoice\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataOpi\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRatepay\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRetry\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRisk\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRiskStandalone\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataSubMerchant\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataTemporaryServices\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataWallets\"\n        }\n\
  \      ],\n      \"description\": \"This field contains additional data, which may be required for a particular modification request.\\n\\nThe additionalData object consists of entries, each of which includes the key and value.\",\n      \"type\": \"object\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account that is used to process the payment.\",\n      \"type\": \"string\"\n    },\n    \"modificationAmount\": {\n      \"description\": \"The amount that needs to be adjusted. The `currency` must match the currency used in authorisation, the `value` must be smaller than or equal to the authorised amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"mpiData\": {\n      \"x-addedInVersion\": \"46\",\n      \"description\": \"Authentication data produced by an MPI (Mastercard SecureCode, Visa Secure, or Cartes Bancaires).\",\n      \"$ref\": \"#/components/schemas/ThreeDSecureData\"\n    },\n    \"originalMerchantReference\": {\n      \"\
  x-addedInVersion\": \"30\",\n      \"description\": \"The original merchant reference to cancel.\",\n      \"type\": \"string\"\n    },\n    \"originalReference\": {\n      \"description\": \"The original pspReference of the payment to modify.\\nThis reference is returned in:\\n* authorisation response\\n* authorisation notification\\n\\n\",\n      \"type\": \"string\"\n    },\n    \"platformChargebackLogic\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Defines how to book chargebacks when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#chargebacks-and-disputes).\",\n      \"$ref\": \"#/components/schemas/PlatformChargebackLogic\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the payment modification. This reference is visible in Customer Area and in reports.\\nMaximum length: 80 characters.\",\n      \"type\": \"string\"\n    },\n    \"splits\": {\n      \"x-addedInVersion\": \"37\",\n\
  \      \"description\": \"An array of objects specifying how the amount should be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#providing-split-information).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Split\"\n      },\n      \"type\": \"array\"\n    },\n    \"tenderReference\": {\n      \"x-addedInVersion\": \"25\",\n      \"description\": \"The transaction reference provided by the PED. For point-of-sale integrations only.\",\n      \"type\": \"string\"\n    },\n    \"uniqueTerminalId\": {\n      \"x-addedInVersion\": \"25\",\n      \"description\": \"Unique terminal ID for the PED that originally processed the request. For point-of-sale integrations only.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"modificationAmount\",\n    \"originalReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-adjust-authorisation-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdjustAuthorisationRequest
---
