---
description: UpdateAccountHolderResponse schema from Adyen API
layout: schema
name: UpdateAccountHolderResponse
properties_list:
- description: The code of the account holder.
  name: accountHolderCode
  type: string
- description: Details of the account holder.
  name: accountHolderDetails
  type: object
- description: The new status of the account holder.
  name: accountHolderStatus
  type: object
- description: The description of the account holder.
  name: description
  type: string
- description: in case the account holder has not been updated, contains account holder fields, that did not pass the validation.
  name: invalidFields
  type: array
- description: The legal entity of the account holder.
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
schema_file: json-schema/accounts-update-account-holder-response-schema.json
slug: accounts-update-account-holder-response
source_filename: accounts-update-account-holder-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-update-account-holder-response-schema.json\",\n  \"title\": \"UpdateAccountHolderResponse\",\n  \"description\": \"UpdateAccountHolderResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"accountHolderDetails\": {\n      \"description\": \"Details of the account holder.\",\n      \"$ref\": \"#/components/schemas/AccountHolderDetails\"\n    },\n    \"accountHolderStatus\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The new status of the account holder.\",\n      \"$ref\": \"#/components/schemas/AccountHolderStatus\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The description of\
  \ the account holder.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"in case the account holder has not been updated, contains account holder fields, that did not pass the validation.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"legalEntity\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The legal entity of the account holder.\",\n      \"enum\": [\n        \"Business\",\n        \"Individual\",\n        \"NonProfit\",\n        \"Partnership\",\n        \"PublicCompany\"\n      ],\n      \"type\": \"string\"\n    },\n    \"primaryCurrency\": {\n      \"x-addedInVersion\": \"5\",\n      \"deprecated\": true,\n      \"description\": \"The three-character [ISO currency code](https://docs.adyen.com/development-resources/currency-codes), with which the prospective account holder primarily deals.\",\n     \
  \ \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request. Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    },\n    \"verification\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The details of KYC Verification of the account holder.\",\n      \"$ref\": \"#/components/schemas/KYCVerificationResult\"\n    },\n    \"verificationProfile\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The identifier of the profile that applies to this entity.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-update-account-holder-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdateAccountHolderResponse
---
