---
description: RecurringDetail schema from Adyen API
layout: schema
name: RecurringDetail
properties_list:
- description: This field contains additional data, which may be returned in a particular response. The additionalData object consists of entries, each of which includes the key and value.
  name: additionalData
  type: object
- description: The alias of the credit card number. Applies only to recurring contracts storing credit card details
  name: alias
  type: string
- description: The alias type of the credit card number. Applies only to recurring contracts storing credit card details.
  name: aliasType
  type: string
- description: A container for bank account data.
  name: bank
  type: object
- description: The billing address.
  name: billingAddress
  type: object
- description: A container for card data.
  name: card
  type: object
- description: Types of recurring contracts.
  name: contractTypes
  type: array
- description: The date when the recurring details were created.
  name: creationDate
  type: string
- description: The `pspReference` of the first recurring payment that created the recurring detail.
  name: firstPspReference
  type: string
- description: An optional descriptive name for this recurring detail.
  name: name
  type: string
- description: Returned in the response if you are not tokenizing with Adyen and are using the Merchant-initiated transactions (MIT) framework from Mastercard or Visa. This contains either the Mastercard Trace ID or
  name: networkTxReference
  type: string
- description: The type or sub-brand of a payment method used, e.g. Visa Debit, Visa Corporate, etc. For more information, refer to [PaymentMethodVariant](https://docs.adyen.com/development-resources/paymentmethodva
  name: paymentMethodVariant
  type: string
- description: The reference that uniquely identifies the recurring detail.
  name: recurringDetailReference
  type: string
- description: The name of the shopper.
  name: shopperName
  type: object
- description: A shopper's social security number (only in countries where it is legal to collect).
  name: socialSecurityNumber
  type: string
- description: ''
  name: tokenDetails
  type: object
- description: The payment method, such as “mc", "visa", "ideal", "paypal".
  name: variant
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-recurring-detail-schema.json
slug: recurring-recurring-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-recurring-detail-schema.json\",\n  \"title\": \"RecurringDetail\",\n  \"description\": \"RecurringDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"x-addedInVersion\": \"5\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"This field contains additional data, which may be returned in a particular response.\\n\\nThe additionalData object consists of entries, each of which includes the key and value.\",\n      \"type\": \"object\"\n    },\n    \"alias\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The alias of the credit card number.\\n\\nApplies only to recurring contracts storing credit card details\",\n      \"type\": \"string\"\n    },\n    \"aliasType\": {\n      \"\
  x-addedInVersion\": \"4\",\n      \"description\": \"The alias type of the credit card number.\\n\\nApplies only to recurring contracts storing credit card details.\",\n      \"type\": \"string\"\n    },\n    \"bank\": {\n      \"description\": \"A container for bank account data.\",\n      \"$ref\": \"#/components/schemas/BankAccount\"\n    },\n    \"billingAddress\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The billing address.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"card\": {\n      \"description\": \"A container for card data.\",\n      \"$ref\": \"#/components/schemas/Card\"\n    },\n    \"contractTypes\": {\n      \"x-addedInVersion\": \"12\",\n      \"description\": \"Types of recurring contracts.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"creationDate\": {\n      \"description\": \"The date when the recurring details were created.\",\n      \"format\": \"date-time\"\
  ,\n      \"type\": \"string\"\n    },\n    \"firstPspReference\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The `pspReference` of the first recurring payment that created the recurring detail.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"An optional descriptive name for this recurring detail.\",\n      \"type\": \"string\"\n    },\n    \"networkTxReference\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Returned in the response if you are not tokenizing with Adyen and are using the Merchant-initiated transactions (MIT) framework from Mastercard or Visa.\\n\\nThis contains either the Mastercard Trace ID or the Visa Transaction ID.\",\n      \"type\": \"string\"\n    },\n    \"paymentMethodVariant\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The  type or sub-brand of a payment method used, e.g. Visa Debit, Visa Corporate, etc. For more information, refer to [PaymentMethodVariant](https://docs.adyen.com/development-resources/paymentmethodvariant).\"\
  ,\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"description\": \"The reference that uniquely identifies the recurring detail.\",\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The name of the shopper.\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"socialSecurityNumber\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"A shopper's social security number (only in countries where it is legal to collect).\",\n      \"type\": \"string\"\n    },\n    \"tokenDetails\": {\n      \"x-addedInVersion\": \"2\",\n      \"$ref\": \"#/components/schemas/TokenDetails\"\n    },\n    \"variant\": {\n      \"description\": \"The payment method, such as \\u201cmc\\\", \\\"visa\\\", \\\"ideal\\\", \\\"paypal\\\".\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"recurringDetailReference\",\n    \"variant\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-recurring-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RecurringDetail
---
