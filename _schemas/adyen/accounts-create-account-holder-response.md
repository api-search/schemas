---
description: CreateAccountHolderResponse schema from Adyen API
layout: schema
name: CreateAccountHolderResponse
properties_list:
- description: The code of a new account created for the account holder.
  name: accountCode
  type: string
- description: The code of the new account holder.
  name: accountHolderCode
  type: string
- description: Details of the new account holder.
  name: accountHolderDetails
  type: object
- description: The status of the new account holder.
  name: accountHolderStatus
  type: object
- description: The description of the new account holder.
  name: description
  type: string
- description: A list of fields that caused the `/createAccountHolder` request to fail.
  name: invalidFields
  type: array
- description: The type of legal entity of the new account holder.
  name: legalEntity
  type: string
- description: The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes), with which the prospective account holder primarily deals.
  name: primaryCurrency
  type: string
- description: The reference of a request. Can be used to uniquely identify the request.
  name: pspReference
  type: string
- description: The result code.
  name: resultCode
  type: string
- description: The details of KYC Verification of the account holder.
  name: verification
  type: object
- description: The identifier of the profile that applies to this entity.
  name: verificationProfile
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-create-account-holder-response-schema.json
slug: accounts-create-account-holder-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-create-account-holder-response-schema.json\",\n  \"title\": \"CreateAccountHolderResponse\",\n  \"description\": \"CreateAccountHolderResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of a new account created for the account holder.\",\n      \"type\": \"string\"\n    },\n    \"accountHolderCode\": {\n      \"description\": \"The code of the new account holder.\",\n      \"type\": \"string\"\n    },\n    \"accountHolderDetails\": {\n      \"description\": \"Details of the new account holder.\",\n      \"$ref\": \"#/components/schemas/AccountHolderDetails\"\n    },\n    \"accountHolderStatus\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The status of the new account holder.\",\n      \"$ref\": \"\
  #/components/schemas/AccountHolderStatus\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The description of the new account holder.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"A list of fields that caused the `/createAccountHolder` request to fail.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"legalEntity\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The type of legal entity of the new account holder.\",\n      \"enum\": [\n        \"Business\",\n        \"Individual\",\n        \"NonProfit\",\n        \"Partnership\",\n        \"PublicCompany\"\n      ],\n      \"type\": \"string\"\n    },\n    \"primaryCurrency\": {\n      \"x-addedInVersion\": \"5\",\n      \"deprecated\": true,\n      \"description\": \"The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes),\
  \ with which the prospective account holder primarily deals.\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request. Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    },\n    \"verification\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The details of KYC Verification of the account holder.\",\n      \"$ref\": \"#/components/schemas/KYCVerificationResult\"\n    },\n    \"verificationProfile\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The identifier of the profile that applies to this entity.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-create-account-holder-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateAccountHolderResponse
---
