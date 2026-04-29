---
description: UpdateAccountHolderRequest schema from Adyen API
layout: schema
name: UpdateAccountHolderRequest
properties_list:
- description: The code of the Account Holder to be updated.
  name: accountHolderCode
  type: string
- description: The details to which the Account Holder should be updated. Required if a processingTier is not provided.
  name: accountHolderDetails
  type: object
- description: A description of the account holder, maximum 256 characters. You can use alphanumeric characters (A-Z, a-z, 0-9), white spaces, and underscores `_`.
  name: description
  type: string
- description: 'The legal entity type of the account holder. This determines the information that should be provided in the request. Possible values: **Business**, **Individual**, or **NonProfit**. * If set to **Busi'
  name: legalEntity
  type: string
- description: The primary three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes), to which the account holder should be updated.
  name: primaryCurrency
  type: string
- description: The processing tier to which the Account Holder should be updated. >The processing tier can not be lowered through this request. >Required if accountHolderDetails are not provided.
  name: processingTier
  type: integer
- description: The identifier of the profile that applies to this entity.
  name: verificationProfile
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-update-account-holder-request-schema.json
slug: accounts-update-account-holder-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-update-account-holder-request-schema.json\",\n  \"title\": \"UpdateAccountHolderRequest\",\n  \"description\": \"UpdateAccountHolderRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the Account Holder to be updated.\",\n      \"type\": \"string\"\n    },\n    \"accountHolderDetails\": {\n      \"description\": \"The details to which the Account Holder should be updated.\\n\\nRequired if a processingTier is not provided.\",\n      \"$ref\": \"#/components/schemas/AccountHolderDetails\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"A description of the account holder, maximum 256 characters. You can use alphanumeric characters (A-Z, a-z, 0-9), white spaces, and underscores\
  \ `_`.\",\n      \"type\": \"string\"\n    },\n    \"legalEntity\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The legal entity type of the account holder. This determines the information that should be provided in the request.\\n\\nPossible values: **Business**, **Individual**, or **NonProfit**.\\n\\n* If set to **Business** or **NonProfit**, then `accountHolderDetails.businessDetails` must be provided, with at least one entry in the `accountHolderDetails.businessDetails.shareholders` list.\\n\\n* If set to **Individual**, then `accountHolderDetails.individualDetails` must be provided.\",\n      \"enum\": [\n        \"Business\",\n        \"Individual\",\n        \"NonProfit\",\n        \"Partnership\",\n        \"PublicCompany\"\n      ],\n      \"type\": \"string\"\n    },\n    \"primaryCurrency\": {\n      \"x-addedInVersion\": \"4\",\n      \"deprecated\": true,\n      \"description\": \"The primary three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes),\
  \ to which the account holder should be updated.\",\n      \"type\": \"string\"\n    },\n    \"processingTier\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The processing tier to which the Account Holder should be updated.\\n>The processing tier can not be lowered through this request.\\n\\n>Required if accountHolderDetails are not provided.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"verificationProfile\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The identifier of the profile that applies to this entity.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-update-account-holder-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdateAccountHolderRequest
---
