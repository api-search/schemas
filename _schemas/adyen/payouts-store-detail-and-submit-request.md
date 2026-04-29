---
description: StoreDetailAndSubmitRequest schema from Adyen API
layout: schema
name: StoreDetailAndSubmitRequest
properties_list:
- description: This field contains additional data, which may be required for a particular request.
  name: additionalData
  type: object
- description: A container object for the payable amount information of the transaction.
  name: amount
  type: object
- description: A container for bank account data. > This field is mandatory if `card` is not provided.
  name: bank
  type: object
- description: The billing address. > The `billingAddress` object is required for cross-border payouts to and from Canada. Include all of the fields within this object.
  name: billingAddress
  type: object
- description: A container for card data. > This field is mandatory if `bank` is not provided.
  name: card
  type: object
- description: 'The date of birth. Format: [ISO-8601](https://www.w3.org/TR/NOTE-datetime); example: YYYY-MM-DD For Paysafecard it must be the same as used when registering the Paysafecard account. > This field is ma'
  name: dateOfBirth
  type: string
- description: The type of the entity the payout is processed for.
  name: entityType
  type: string
- description: An integer value that is added to the normal fraud score. The value can be either positive or negative.
  name: fraudOffset
  type: integer
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: The shopper's nationality. A valid value is an ISO 2-character country code (e.g. 'NL').
  name: nationality
  type: string
- description: A container for the type of recurring contract to be retrieved. The recurring.contract must be set to `PAYOUT`
  name: recurring
  type: object
- description: 'The merchant reference for this payment. This reference will be used in all communication to the merchant about the status of the payout. Although it is a good idea to make sure it is unique, this is '
  name: reference
  type: string
- description: The name of the brand to make a payout to. For Paysafecard it must be set to `paysafecard`.
  name: selectedBrand
  type: string
- description: The shopper's email address.
  name: shopperEmail
  type: string
- description: The shopper's name. When the `entityType` is `Company`, the `shopperName.lastName` must contain the company name.
  name: shopperName
  type: object
- description: The shopper's reference for the payment transaction.
  name: shopperReference
  type: string
- description: The description of this payout. This description is shown on the bank statement of the shopper (if this is supported by the chosen payment method).
  name: shopperStatement
  type: string
- description: The shopper's social security number.
  name: socialSecurityNumber
  type: string
- description: The shopper's phone number.
  name: telephoneNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payouts-store-detail-and-submit-request-schema.json
slug: payouts-store-detail-and-submit-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-store-detail-and-submit-request-schema.json\",\n  \"title\": \"StoreDetailAndSubmitRequest\",\n  \"description\": \"StoreDetailAndSubmitRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"This field contains additional data, which may be required for a particular request.\",\n      \"type\": \"object\"\n    },\n    \"amount\": {\n      \"description\": \"A container object for the payable amount information of the transaction.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"bank\": {\n      \"description\": \"A container for bank account data.\\n> This field is mandatory if `card` is not provided.\",\n      \"$ref\": \"#/components/schemas/BankAccount\"\
  \n    },\n    \"billingAddress\": {\n      \"x-addedInVersion\": \"18\",\n      \"description\": \"The billing address.\\n\\n> The `billingAddress` object is required for cross-border payouts to and from Canada. Include all of the fields within this object.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"card\": {\n      \"description\": \"A container for card data.\\n> This field is mandatory if `bank` is not provided.\",\n      \"$ref\": \"#/components/schemas/Card\"\n    },\n    \"dateOfBirth\": {\n      \"x-addedInVersion\": \"24\",\n      \"description\": \"The date of birth.\\nFormat: [ISO-8601](https://www.w3.org/TR/NOTE-datetime); example: YYYY-MM-DD\\nFor Paysafecard it must be the same as used when registering the Paysafecard account.\\n> This field is mandatory for natural persons.\",\n      \"format\": \"date\",\n      \"type\": \"string\"\n    },\n    \"entityType\": {\n      \"x-addedInVersion\": \"24\",\n      \"description\": \"The type of the entity\
  \ the payout is processed for.\",\n      \"enum\": [\n        \"NaturalPerson\",\n        \"Company\"\n      ],\n      \"type\": \"string\"\n    },\n    \"fraudOffset\": {\n      \"description\": \"An integer value that is added to the normal fraud score. The value can be either positive or negative.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"nationality\": {\n      \"x-addedInVersion\": \"24\",\n      \"description\": \"The shopper's nationality.\\n\\nA valid value is an ISO 2-character country code (e.g. 'NL').\",\n      \"maxLength\": 2,\n      \"type\": \"string\"\n    },\n    \"recurring\": {\n      \"description\": \"A container for the type of recurring contract to be retrieved.\\n\\nThe recurring.contract must be set to `PAYOUT`\",\n      \"$ref\": \"#/components/schemas/Recurring\"\
  \n    },\n    \"reference\": {\n      \"description\": \"The merchant reference for this payment. This reference will be used in all communication to the merchant about the status of the payout. Although it is a good idea to make sure it is unique, this is not a requirement.\",\n      \"type\": \"string\"\n    },\n    \"selectedBrand\": {\n      \"x-addedInVersion\": \"24\",\n      \"description\": \"The name of the brand to make a payout to.\\n\\nFor Paysafecard it must be set to `paysafecard`.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper's email address.\",\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"x-addedInVersion\": \"24\",\n      \"description\": \"The shopper's name.\\n\\nWhen the `entityType` is `Company`, the `shopperName.lastName` must contain the company name.\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"shopperReference\": {\n      \"description\": \"The shopper's reference\
  \ for the payment transaction.\",\n      \"type\": \"string\"\n    },\n    \"shopperStatement\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The description of this payout. This description is shown on the bank statement of the shopper (if this is supported by the chosen payment method).\",\n      \"type\": \"string\"\n    },\n    \"socialSecurityNumber\": {\n      \"x-addedInVersion\": \"24\",\n      \"description\": \"The shopper's social security number.\",\n      \"type\": \"string\"\n    },\n    \"telephoneNumber\": {\n      \"x-addedInVersion\": \"52\",\n      \"description\": \"The shopper's phone number.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"shopperEmail\",\n    \"shopperReference\",\n    \"recurring\",\n    \"dateOfBirth\",\n    \"nationality\",\n    \"entityType\",\n    \"reference\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-store-detail-and-submit-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoreDetailAndSubmitRequest
---
