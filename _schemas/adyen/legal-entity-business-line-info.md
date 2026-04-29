---
description: BusinessLineInfo schema from Adyen API
layout: schema
name: BusinessLineInfo
properties_list:
- description: 'The capability for which you are creating the business line. Possible values: **receivePayments**, **receiveFromPlatformPayments**, **issueBankAccount**'
  name: capability
  type: string
- description: 'A code that represents the [industry of the legal entity](https://docs.adyen.com/marketplaces-and-platforms/verification-requirements/reference-additional-products/#list-industry-codes). For example, '
  name: industryCode
  type: string
- description: Unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/legalEntities__resParam_id) that owns the business line.
  name: legalEntityId
  type: string
- description: 'A list of channels where goods or services are sold. Possible values: **pos**, **posMoto**, **eCommerce**, **ecomMoto**, **payByLink**. Required only in combination with the `service` **paymentProcess'
  name: salesChannels
  type: array
- description: 'The service for which you are creating the business line. Possible values: * **paymentProcessing** * **banking**'
  name: service
  type: string
- description: Contains information about the source of your user's funds. Required only for the `service` **banking**.
  name: sourceOfFunds
  type: object
- description: List of website URLs where your user's goods or services are sold. When this is required for a service but your user does not have an online presence, provide the reason in the `webDataExemption` obje
  name: webData
  type: array
- description: The reason why the web data is not provided.
  name: webDataExemption
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-business-line-info-schema.json
slug: legal-entity-business-line-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-business-line-info-schema.json\",\n  \"title\": \"BusinessLineInfo\",\n  \"description\": \"BusinessLineInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capability\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"3\",\n      \"x-deprecatedMessage\": \"Use `service` instead.\",\n      \"description\": \"The capability for which you are creating the business line.\\n\\nPossible values: **receivePayments**, **receiveFromPlatformPayments**, **issueBankAccount**\",\n      \"enum\": [\n        \"receivePayments\",\n        \"receiveFromPlatformPayments\",\n        \"issueBankAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"industryCode\": {\n      \"description\": \"A code that represents the [industry of the legal entity](https://docs.adyen.com/marketplaces-and-platforms/verification-requirements/reference-additional-products/#list-industry-codes).\
  \ For example, **4431A** for computer software stores.\",\n      \"type\": \"string\"\n    },\n    \"legalEntityId\": {\n      \"description\": \"Unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/legalEntities__resParam_id) that owns the business line.\",\n      \"type\": \"string\"\n    },\n    \"salesChannels\": {\n      \"description\": \"A list of channels where goods or services are sold.\\n\\nPossible values: **pos**, **posMoto**, **eCommerce**, **ecomMoto**, **payByLink**.\\n\\nRequired only in combination with the `service` **paymentProcessing**.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"service\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The service for which you are creating the business line.\\n\\n\\n\\nPossible values:\\n*  **paymentProcessing**\\n*  **banking**\\n\\n\",\n      \"enum\": [\n        \"paymentProcessing\",\n        \"banking\"\
  \n      ],\n      \"type\": \"string\"\n    },\n    \"sourceOfFunds\": {\n      \"description\": \"Contains information about the source of your user's funds. Required only for the `service` **banking**.\",\n      \"$ref\": \"#/components/schemas/SourceOfFunds\"\n    },\n    \"webData\": {\n      \"description\": \"List of website URLs where your user's goods or services are sold. When this is required for a service but your user does not have an online presence, provide the reason in the `webDataExemption` object.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/WebData\"\n      },\n      \"type\": \"array\"\n    },\n    \"webDataExemption\": {\n      \"description\": \"The reason why the web data is not provided.\",\n      \"$ref\": \"#/components/schemas/WebDataExemption\"\n    }\n  },\n  \"required\": [\n    \"service\",\n    \"industryCode\",\n    \"legalEntityId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-business-line-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BusinessLineInfo
---
