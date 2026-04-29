---
description: SubmitRequest schema from Adyen API
layout: schema
name: SubmitRequest
properties_list:
- description: This field contains additional data, which may be required for a particular request.
  name: additionalData
  type: object
- description: A container object for the payable amount information of the transaction.
  name: amount
  type: object
- description: 'The date of birth. Format: ISO-8601; example: YYYY-MM-DD For Paysafecard it must be the same as used when registering the Paysafecard account. > This field is mandatory for natural persons. > This fie'
  name: dateOfBirth
  type: string
- description: 'The type of the entity the payout is processed for. Allowed values: * NaturalPerson * Company > This field is required to update the existing `entityType` that is associated with this recurring contra'
  name: entityType
  type: string
- description: An integer value that is added to the normal fraud score. The value can be either positive or negative.
  name: fraudOffset
  type: integer
- description: The merchant account identifier you want to process the transaction request with.
  name: merchantAccount
  type: string
- description: The shopper's nationality. A valid value is an ISO 2-character country code (e.g. 'NL'). > This field is required to update the existing nationality that is associated with this recurring contract.
  name: nationality
  type: string
- description: A container for the type of recurring contract to be retrieved. The `recurring.contract` must be set to "PAYOUT".
  name: recurring
  type: object
- description: The merchant reference for this payout. This reference will be used in all communication to the merchant about the status of the payout. Although it is a good idea to make sure it is unique, this is n
  name: reference
  type: string
- description: This is the `recurringDetailReference` you want to use for this payout. You can use the value LATEST to select the most recently used recurring detail.
  name: selectedRecurringDetailReference
  type: string
- description: The shopper's email address.
  name: shopperEmail
  type: string
- description: The shopper's name. In case the `entityType` is `Company`, the `shopperName.lastName` must contain the company name. > This field is required to update the existing `shopperName` associated with a rec
  name: shopperName
  type: object
- description: The shopper's reference for the payout transaction.
  name: shopperReference
  type: string
- description: The description of this payout. This description is shown on the bank statement of the shopper (if this is supported by the chosen payment method).
  name: shopperStatement
  type: string
- description: The shopper's social security number.
  name: socialSecurityNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payouts-submit-request-schema.json
slug: payouts-submit-request
source_filename: payouts-submit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-submit-request-schema.json\",\n  \"title\": \"SubmitRequest\",\n  \"description\": \"SubmitRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"This field contains additional data, which may be required for a particular request.\",\n      \"type\": \"object\"\n    },\n    \"amount\": {\n      \"description\": \"A container object for the payable amount information of the transaction.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"dateOfBirth\": {\n      \"x-addedInVersion\": \"24\",\n      \"description\": \"The date of birth.\\nFormat: ISO-8601; example: YYYY-MM-DD\\n\\nFor Paysafecard it must be the same as used when registering the\
  \ Paysafecard account.\\n\\n> This field is mandatory for natural persons. \\n> This field is required to update the existing `dateOfBirth` that is associated with this recurring contract.\",\n      \"format\": \"date\",\n      \"type\": \"string\"\n    },\n    \"entityType\": {\n      \"x-addedInVersion\": \"24\",\n      \"description\": \"The type of the entity the payout is processed for.\\n\\nAllowed values:\\n* NaturalPerson\\n* Company\\n> This field is required to update the existing `entityType` that is associated with this recurring contract.\",\n      \"enum\": [\n        \"NaturalPerson\",\n        \"Company\"\n      ],\n      \"type\": \"string\"\n    },\n    \"fraudOffset\": {\n      \"description\": \"An integer value that is added to the normal fraud score. The value can be either positive or negative.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier you want to process\
  \ the transaction request with.\",\n      \"type\": \"string\"\n    },\n    \"nationality\": {\n      \"x-addedInVersion\": \"24\",\n      \"description\": \"The shopper's nationality.\\n\\nA valid value is an ISO 2-character country code (e.g. 'NL').\\n\\n> This field is required to update the existing nationality that is associated with this recurring contract.\",\n      \"type\": \"string\"\n    },\n    \"recurring\": {\n      \"description\": \"A container for the type of recurring contract to be retrieved.\\n\\nThe `recurring.contract` must be set to \\\"PAYOUT\\\".\",\n      \"$ref\": \"#/components/schemas/Recurring\"\n    },\n    \"reference\": {\n      \"description\": \"The merchant reference for this payout. This reference will be used in all communication to the merchant about the status of the payout. Although it is a good idea to make sure it is unique, this is not a requirement.\",\n      \"type\": \"string\"\n    },\n    \"selectedRecurringDetailReference\": {\n      \"\
  description\": \"This is the `recurringDetailReference` you want to use for this payout.\\n\\nYou can use the value LATEST to select the most recently used recurring detail.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper's email address.\",\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"x-addedInVersion\": \"24\",\n      \"description\": \"The shopper's name.\\n\\nIn case the `entityType` is `Company`, the `shopperName.lastName` must contain the company name.\\n\\n> This field is required to update the existing `shopperName` associated with a recurring contract.\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"shopperReference\": {\n      \"description\": \"The shopper's reference for the payout transaction.\",\n      \"type\": \"string\"\n    },\n    \"shopperStatement\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The description of this payout. This description is shown on\
  \ the bank statement of the shopper (if this is supported by the chosen payment method).\",\n      \"type\": \"string\"\n    },\n    \"socialSecurityNumber\": {\n      \"x-addedInVersion\": \"24\",\n      \"description\": \"The shopper's social security number.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"reference\",\n    \"amount\",\n    \"shopperEmail\",\n    \"shopperReference\",\n    \"recurring\",\n    \"selectedRecurringDetailReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-submit-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SubmitRequest
---
