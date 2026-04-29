---
description: IssuedCard schema from Adyen API
layout: schema
name: IssuedCard
properties_list:
- description: The authorisation type. For example, **defaultAuthorisation**, **preAuthorisation**, **finalAuthorisation**
  name: authorisationType
  type: string
- description: 'Indicates the method used for entering the PAN to initiate a transaction. Possible values: **manual**, **chip**, **magstripe**, **contactless**, **cof**, **ecommerce**, **token**.'
  name: panEntryMode
  type: string
- description: Contains information about how the payment was processed. For example, **ecommerce** for online or **pos** for in-person payments.
  name: processingType
  type: string
- description: If you are using relayed authorisation, this object contains information from the relayed authorisation response from your server.
  name: relayedAuthorisationData
  type: object
- description: The identifier of the original payment provided by the scheme. The Id could be alphanumeric or numeric depending on the scheme. The schemeTraceID should be referring to an original schemeUniqueTransac
  name: schemeTraceId
  type: string
- description: The unique identifier created by the scheme. The ID could be alphanumeric or numeric depending on the scheme.
  name: schemeUniqueTransactionId
  type: string
- description: '**issuedCard**'
  name: type
  type: string
- description: The evaluation of the validation facts. See [validation checks](https://docs.adyen.com/issuing/validation-checks) for more information.
  name: validationFacts
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-issued-card-schema.json
slug: transfer-webhooks-issued-card
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-issued-card-schema.json\",\n  \"title\": \"IssuedCard\",\n  \"description\": \"IssuedCard schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorisationType\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The authorisation type. For example, **defaultAuthorisation**, **preAuthorisation**, **finalAuthorisation**\",\n      \"type\": \"string\"\n    },\n    \"panEntryMode\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"Indicates the method used for entering the PAN to initiate a transaction.\\n\\nPossible values: **manual**, **chip**, **magstripe**, **contactless**, **cof**, **ecommerce**, **token**.\",\n      \"enum\": [\n        \"chip\",\n        \"cof\",\n        \"contactless\",\n        \"ecommerce\",\n        \"magstripe\",\n\
  \        \"manual\",\n        \"token\"\n      ],\n      \"type\": \"string\"\n    },\n    \"processingType\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"Contains information about how the payment was processed. For example, **ecommerce** for online or **pos** for in-person payments.\",\n      \"enum\": [\n        \"atmWithdraw\",\n        \"balanceInquiry\",\n        \"ecommerce\",\n        \"moto\",\n        \"pos\",\n        \"purchaseWithCashback\",\n        \"recurring\",\n        \"token\"\n      ],\n      \"type\": \"string\"\n    },\n    \"relayedAuthorisationData\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"If you are using relayed authorisation, this object contains information from the relayed authorisation response from your server.\",\n      \"$ref\": \"#/components/schemas/RelayedAuthorisationData\"\n    },\n    \"schemeTraceId\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The identifier of the original payment\
  \ provided by the scheme. The Id could be alphanumeric or numeric depending on the scheme. The schemeTraceID should be referring to an original schemeUniqueTransactionID provided in an earlier payment (not necessarily processed by Adyen). Instances of available schemeTraceId is authAdjustment or recurring payments.\",\n      \"type\": \"string\"\n    },\n    \"schemeUniqueTransactionId\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The unique identifier created by the scheme. The ID could be alphanumeric or numeric depending on the scheme.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"issuedCard\",\n      \"description\": \"**issuedCard**\",\n      \"enum\": [\n        \"issuedCard\"\n      ],\n      \"type\": \"string\"\n    },\n    \"validationFacts\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The evaluation of the validation facts. See [validation checks](https://docs.adyen.com/issuing/validation-checks) for more\
  \ information.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransferNotificationValidationFact\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-issued-card-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: IssuedCard
---
