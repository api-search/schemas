---
description: StoredPaymentMethodResource schema from Adyen API
layout: schema
name: StoredPaymentMethodResource
properties_list:
- description: The brand of the card.
  name: brand
  type: string
- description: The month the card expires.
  name: expiryMonth
  type: string
- description: The last two digits of the year the card expires. For example, **22** for the year 2022.
  name: expiryYear
  type: string
- description: The response code returned by an external system (for example after a provisioning operation).
  name: externalResponseCode
  type: string
- description: The token reference of a linked token in an external system (for example a network token reference).
  name: externalTokenReference
  type: string
- description: The unique payment method code.
  name: holderName
  type: string
- description: The IBAN of the bank account.
  name: iban
  type: string
- description: A unique identifier of this stored payment method.
  name: id
  type: string
- description: The name of the issuer of token or card.
  name: issuerName
  type: string
- description: The last four digits of the PAN.
  name: lastFour
  type: string
- description: The display name of the stored payment method.
  name: name
  type: string
- description: Returned in the response if you are not tokenizing with Adyen and are using the Merchant-initiated transactions (MIT) framework from Mastercard or Visa. This contains either the Mastercard Trace ID or
  name: networkTxReference
  type: string
- description: The name of the bank account holder.
  name: ownerName
  type: string
- description: The shopper’s email address.
  name: shopperEmail
  type: string
- description: 'Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters. > Your reference must not include personally identifiable information (PII), for exam'
  name: shopperReference
  type: string
- description: 'Defines a recurring payment type. Allowed values: * `Subscription` – A transaction for a fixed or variable amount, which follows a fixed schedule. * `CardOnFile` – With a card-on-file (CoF) transactio'
  name: supportedRecurringProcessingModels
  type: array
- description: The type of payment method.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-stored-payment-method-resource-schema.json
slug: checkout-stored-payment-method-resource
source_filename: checkout-stored-payment-method-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-stored-payment-method-resource-schema.json\",\n  \"title\": \"StoredPaymentMethodResource\",\n  \"description\": \"StoredPaymentMethodResource schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"description\": \"The brand of the card.\",\n      \"type\": \"string\"\n    },\n    \"expiryMonth\": {\n      \"description\": \"The month the card expires.\",\n      \"type\": \"string\"\n    },\n    \"expiryYear\": {\n      \"description\": \"The last two digits of the year the card expires. For example, **22** for the year 2022.\",\n      \"type\": \"string\"\n    },\n    \"externalResponseCode\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The response code returned by an external system (for example after a provisioning operation).\",\n    \
  \  \"type\": \"string\"\n    },\n    \"externalTokenReference\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The token reference of a linked token in an external system (for example a network token reference).\",\n      \"type\": \"string\"\n    },\n    \"holderName\": {\n      \"description\": \"The unique payment method code.\",\n      \"type\": \"string\"\n    },\n    \"iban\": {\n      \"description\": \"The IBAN of the bank account.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"A unique identifier of this stored payment method.\",\n      \"type\": \"string\"\n    },\n    \"issuerName\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The name of the issuer of token or card.\",\n      \"type\": \"string\"\n    },\n    \"lastFour\": {\n      \"description\": \"The last four digits of the PAN.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The display name of the stored payment\
  \ method.\",\n      \"type\": \"string\"\n    },\n    \"networkTxReference\": {\n      \"description\": \"Returned in the response if you are not tokenizing with Adyen and are using the Merchant-initiated transactions (MIT) framework from Mastercard or Visa.\\n\\nThis contains either the Mastercard Trace ID or the Visa Transaction ID.\",\n      \"type\": \"string\"\n    },\n    \"ownerName\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"The name of the bank account holder.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper\\u2019s email address.\",\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters.\\n> Your reference must not include personally identifiable information (PII), for example name or email address.\",\n      \"maxLength\": 256,\n      \"minLength\": 3,\n\
  \      \"type\": \"string\"\n    },\n    \"supportedRecurringProcessingModels\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Defines a recurring payment type.\\nAllowed values:\\n* `Subscription` \\u2013 A transaction for a fixed or variable amount, which follows a fixed schedule.\\n* `CardOnFile` \\u2013 With a card-on-file (CoF) transaction, card details are stored to enable one-click or omnichannel journeys, or simply to streamline the checkout process. Any subscription not following a fixed schedule is also considered a card-on-file transaction.\\n* `UnscheduledCardOnFile` \\u2013 An unscheduled card-on-file (UCoF) transaction is a transaction that occurs on a non-fixed schedule and/or have variable amounts. For example, automatic top-ups when a cardholder's balance drops below a certain amount.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"description\": \"The type of payment method.\"\
  ,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-stored-payment-method-resource-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredPaymentMethodResource
---
