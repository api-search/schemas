---
description: CapitalGrant schema from Adyen API
layout: schema
name: CapitalGrant
properties_list:
- description: An object containing the amount of the grant, in [minor units](https://docs.adyen.com/development-resources/currency-codes).
  name: amount
  type: object
- description: An object containing the details of the existing grant.
  name: balances
  type: object
- description: An object containing the details of the receiving party of the grant. Setting either an `accountHolderId`, `balanceAccountId`, or both is required.
  name: counterparty
  type: object
- description: An object containing the fee currency and value, in [minor units](https://docs.adyen.com/development-resources/currency-codes).
  name: fee
  type: object
- description: The identifier of the grant account used for the grant.
  name: grantAccountId
  type: string
- description: The identifier of the grant offer that has been selected and from which the grant details will be used.
  name: grantOfferId
  type: string
- description: The identifier of the grant reference.
  name: id
  type: string
- description: An object containing the details of the 30-day repayment threshold.
  name: repayment
  type: object
- description: 'The current status of the grant. Possible values: **Pending**, **Active**, **Repaid**.'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-capital-grant-schema.json
slug: transfers-capital-grant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-capital-grant-schema.json\",\n  \"title\": \"CapitalGrant\",\n  \"description\": \"CapitalGrant schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"An object containing the amount of the grant, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"balances\": {\n      \"description\": \"An object containing the details of the existing grant.\",\n      \"$ref\": \"#/components/schemas/CapitalBalance\"\n    },\n    \"counterparty\": {\n      \"description\": \"An object containing the details of the receiving party of the grant. Setting either an `accountHolderId`, `balanceAccountId`, or both is required.\",\n      \"$ref\": \"#/components/schemas/Counterparty\"\
  \n    },\n    \"fee\": {\n      \"description\": \"An object containing the fee currency and value, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\",\n      \"$ref\": \"#/components/schemas/Fee\"\n    },\n    \"grantAccountId\": {\n      \"description\": \"The identifier of the grant account used for the grant.\",\n      \"type\": \"string\"\n    },\n    \"grantOfferId\": {\n      \"description\": \"The identifier of the grant offer that has been selected and from which the grant details will be used.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The identifier of the grant reference.\",\n      \"type\": \"string\"\n    },\n    \"repayment\": {\n      \"description\": \"An object containing the details of the 30-day repayment threshold.\",\n      \"$ref\": \"#/components/schemas/Repayment\"\n    },\n    \"status\": {\n      \"description\": \"The current status of the grant. Possible values: **Pending**, **Active**, **Repaid**.\"\
  ,\n      \"enum\": [\n        \"Pending\",\n        \"Active\",\n        \"Repaid\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"grantAccountId\",\n    \"grantOfferId\",\n    \"id\",\n    \"status\",\n    \"balances\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-capital-grant-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapitalGrant
---
