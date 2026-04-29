---
description: CreateAccountHolderRequest schema from Adyen API
layout: schema
name: CreateAccountHolderRequest
properties_list:
- description: Your unique identifier for the prospective account holder. The length must be between three (3) and fifty (50) characters long. Only letters, digits, and hyphens (-) are allowed.
  name: accountHolderCode
  type: string
- description: The details of the prospective account holder.
  name: accountHolderDetails
  type: object
- description: If set to **true**, an account with the default options is automatically created for the account holder. By default, this field is set to **true**.
  name: createDefaultAccount
  type: boolean
- description: A description of the prospective account holder, maximum 256 characters. You can use alphanumeric characters (A-Z, a-z, 0-9), white spaces, and underscores `_`.
  name: description
  type: string
- description: 'The legal entity type of the account holder. This determines the information that should be provided in the request. Possible values: **Business**, **Individual**, or **NonProfit**. * If set to **Busi'
  name: legalEntity
  type: string
- description: The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes), with which the prospective account holder primarily deals.
  name: primaryCurrency
  type: string
- description: The starting [processing tier](https://docs.adyen.com/marketplaces-and-platforms/classic/onboarding-and-verification/precheck-kyc-information) for the prospective account holder.
  name: processingTier
  type: integer
- description: The identifier of the profile that applies to this entity.
  name: verificationProfile
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-create-account-holder-request-schema.json
slug: accounts-create-account-holder-request
source_filename: accounts-create-account-holder-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-create-account-holder-request-schema.json\",\n  \"title\": \"CreateAccountHolderRequest\",\n  \"description\": \"CreateAccountHolderRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"Your unique identifier for the prospective account holder.\\nThe length must be between three (3) and fifty (50) characters long. Only letters, digits, and hyphens (-) are allowed.\",\n      \"type\": \"string\"\n    },\n    \"accountHolderDetails\": {\n      \"description\": \"The details of the prospective account holder.\",\n      \"$ref\": \"#/components/schemas/AccountHolderDetails\"\n    },\n    \"createDefaultAccount\": {\n      \"description\": \"If set to **true**, an account with the default options is automatically created for the\
  \ account holder.\\nBy default, this field is set to **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"A description of the prospective account holder, maximum 256 characters. You can use alphanumeric characters (A-Z, a-z, 0-9), white spaces, and underscores `_`.\",\n      \"type\": \"string\"\n    },\n    \"legalEntity\": {\n      \"description\": \"The legal entity type of the account holder. This determines the information that should be provided in the request.\\n\\nPossible values: **Business**, **Individual**, or **NonProfit**.\\n\\n* If set to **Business** or **NonProfit**, then `accountHolderDetails.businessDetails` must be provided, with at least one entry in the `accountHolderDetails.businessDetails.shareholders` list.\\n\\n* If set to **Individual**, then `accountHolderDetails.individualDetails` must be provided.\",\n      \"enum\": [\n        \"Business\",\n        \"Individual\",\n      \
  \  \"NonProfit\",\n        \"Partnership\",\n        \"PublicCompany\"\n      ],\n      \"type\": \"string\"\n    },\n    \"primaryCurrency\": {\n      \"x-addedInVersion\": \"4\",\n      \"deprecated\": true,\n      \"description\": \"The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes), with which the prospective account holder primarily deals.\",\n      \"type\": \"string\"\n    },\n    \"processingTier\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The starting [processing tier](https://docs.adyen.com/marketplaces-and-platforms/classic/onboarding-and-verification/precheck-kyc-information) for the prospective account holder.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"verificationProfile\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The identifier of the profile that applies to this entity.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\"\
  ,\n    \"legalEntity\",\n    \"accountHolderDetails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-create-account-holder-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateAccountHolderRequest
---
