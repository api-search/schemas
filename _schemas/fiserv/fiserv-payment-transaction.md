---
description: Schema representing a payment transaction across Fiserv payment processing APIs including CommerceHub and CardPointe Gateway.
layout: schema
name: Fiserv Payment Transaction
properties_list:
- description: The unique identifier assigned to the transaction by the gateway.
  name: transactionId
  type: string
- description: The merchant-assigned order identifier.
  name: orderId
  type: string
- description: The merchant identifier.
  name: merchantId
  type: string
- description: The type of transaction.
  name: transactionType
  type: string
- description: The current state of the transaction.
  name: transactionState
  type: string
- description: ''
  name: amount
  type: object
- description: The ISO 4217 three-letter currency code.
  name: currency
  type: string
- description: ''
  name: paymentSource
  type: object
- description: ''
  name: processorResponse
  type: object
- description: ''
  name: billingAddress
  type: object
- description: The timestamp when the transaction was created.
  name: createdAt
  type: string
- description: The timestamp when the transaction was last updated.
  name: updatedAt
  type: string
- description: Whether the transaction was captured immediately.
  name: captureFlag
  type: boolean
- description: The date the transaction was settled.
  name: settlementDate
  type: string
provider_name: Fiserv
provider_slug: fiserv
schema_file: json-schema/fiserv-payment-transaction-schema.json
slug: fiserv-payment-transaction
source_filename: fiserv-payment-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.fiserv.com/schemas/fiserv/payment-transaction.json\",\n  \"title\": \"Fiserv Payment Transaction\",\n  \"description\": \"Schema representing a payment transaction across Fiserv payment processing APIs including CommerceHub and CardPointe Gateway.\",\n  \"type\": \"object\",\n  \"required\": [\"transactionId\", \"amount\", \"currency\", \"transactionType\", \"transactionState\"],\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier assigned to the transaction by the gateway.\"\n    },\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant-assigned order identifier.\"\n    },\n    \"merchantId\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant identifier.\"\n    },\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"enum\": [\"CHARGE\", \"\
  AUTHORIZATION\", \"CAPTURE\", \"REFUND\", \"VOID\", \"VERIFICATION\"],\n      \"description\": \"The type of transaction.\"\n    },\n    \"transactionState\": {\n      \"type\": \"string\",\n      \"enum\": [\"AUTHORIZED\", \"CAPTURED\", \"SETTLED\", \"REFUNDED\", \"VOIDED\", \"DECLINED\", \"PENDING\"],\n      \"description\": \"The current state of the transaction.\"\n    },\n    \"amount\": {\n      \"$ref\": \"#/$defs/Amount\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"The ISO 4217 three-letter currency code.\"\n    },\n    \"paymentSource\": {\n      \"$ref\": \"#/$defs/PaymentSource\"\n    },\n    \"processorResponse\": {\n      \"$ref\": \"#/$defs/ProcessorResponse\"\n    },\n    \"billingAddress\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the transaction was created.\"\n\
  \    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the transaction was last updated.\"\n    },\n    \"captureFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the transaction was captured immediately.\"\n    },\n    \"settlementDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the transaction was settled.\"\n    }\n  },\n  \"$defs\": {\n    \"Amount\": {\n      \"type\": \"object\",\n      \"description\": \"A monetary amount.\",\n      \"required\": [\"total\"],\n      \"properties\": {\n        \"total\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"The total amount.\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"The ISO 4217 currency code.\"\n        }\n      }\n    },\n    \"PaymentSource\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"The payment source used for the transaction.\",\n      \"properties\": {\n        \"sourceType\": {\n          \"type\": \"string\",\n          \"enum\": [\"PaymentCard\", \"PaymentToken\", \"PaymentSession\", \"GooglePay\", \"ApplePay\", \"BankAccount\"],\n          \"description\": \"The type of payment source.\"\n        },\n        \"cardBrand\": {\n          \"type\": \"string\",\n          \"enum\": [\"VISA\", \"MASTERCARD\", \"AMEX\", \"DISCOVER\", \"JCB\", \"DINERS\"],\n          \"description\": \"The card brand.\"\n        },\n        \"maskedCardNumber\": {\n          \"type\": \"string\",\n          \"pattern\": \"^\\\\*{4,}\\\\d{4}$\",\n          \"description\": \"The masked card number showing only the last four digits.\"\n        },\n        \"expirationMonth\": {\n          \"type\": \"string\",\n          \"pattern\": \"^\\\\d{2}$\",\n          \"description\": \"The card expiration month in MM format.\"\n   \
  \     },\n        \"expirationYear\": {\n          \"type\": \"string\",\n          \"pattern\": \"^\\\\d{4}$\",\n          \"description\": \"The card expiration year in YYYY format.\"\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"The payment token if tokenized.\"\n        }\n      }\n    },\n    \"ProcessorResponse\": {\n      \"type\": \"object\",\n      \"description\": \"The response from the payment processor.\",\n      \"properties\": {\n        \"approvalStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"APPROVED\", \"DECLINED\", \"PROCESSING_FAILED\", \"RETRY\"],\n          \"description\": \"The approval status.\"\n        },\n        \"approvalCode\": {\n          \"type\": \"string\",\n          \"description\": \"The issuer approval code.\"\n        },\n        \"responseCode\": {\n          \"type\": \"string\",\n          \"description\": \"The processor response code.\"\n        },\n        \"responseMessage\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The human-readable response message.\"\n        },\n        \"avsResponseCode\": {\n          \"type\": \"string\",\n          \"description\": \"The Address Verification System response code.\"\n        },\n        \"cvvResponseCode\": {\n          \"type\": \"string\",\n          \"description\": \"The Card Verification Value response code.\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A physical or billing address.\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\",\n          \"maxLength\": 255,\n          \"description\": \"Address line 1.\"\n        },\n        \"line2\": {\n          \"type\": \"string\",\n          \"maxLength\": 255,\n          \"description\": \"Address line 2.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"maxLength\": 100,\n          \"description\": \"The city.\"\n   \
  \     },\n        \"state\": {\n          \"type\": \"string\",\n          \"maxLength\": 100,\n          \"description\": \"The state or province.\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\",\n          \"maxLength\": 20,\n          \"description\": \"The postal or ZIP code.\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"description\": \"The ISO 3166-1 alpha-2 country code.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fiserv/refs/heads/main/json-schema/fiserv-payment-transaction-schema.json
tags:
- Banking
- Financial
- Payments
- Wealth Management
title: Fiserv Payment Transaction
---
