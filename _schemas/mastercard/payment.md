---
description: A payment transaction processed through the Mastercard network, representing a transfer of funds between a payer and payee. Applicable across Mastercard Send, Account to Account Commerce, Bill Pay, and checkout solutions.
layout: schema
name: Mastercard Payment
properties_list:
- description: Unique identifier for the payment, generated using UUID logic to unambiguously link request and response messages.
  name: paymentId
  type: string
- description: Classification of the payment indicating its purpose and processing path.
  name: paymentType
  type: string
- description: Payment amount without decimal separators. The number of implied decimal places depends on the currency. For example, 10350 in USD represents $103.50.
  name: amount
  type: string
- description: ISO 4217 numeric currency code for the payment amount.
  name: currency
  type: string
- description: Current status of the payment in its lifecycle.
  name: status
  type: string
- description: Timestamp of the payment initiation in ISO 8601 format with timezone offset.
  name: timestamp
  type: string
- description: The party initiating or funding the payment.
  name: sender
  type: object
- description: The party receiving the payment funds.
  name: recipient
  type: object
- description: Primary Account Number (PAN) of the card used for the payment. Must pass Luhn algorithm validation.
  name: cardNumber
  type: string
- description: Payment token representing the card number for tokenized transactions (MDES).
  name: tokenNumber
  type: string
- description: Card acceptor or merchant unique identification number assigned by the acquirer.
  name: merchantId
  type: string
- description: Name of the card acceptor or merchant.
  name: merchantName
  type: string
- description: Four-digit ISO 18245 Merchant Category Code (MCC) classifying the type of business.
  name: merchantCategoryCode
  type: string
- description: Interbank Card Association (ICA) number of the acquiring institution.
  name: acquirerId
  type: string
- description: ICA number of the issuer or acquirer initiating the request.
  name: icaNumber
  type: string
- description: Authorization code returned by the issuer for an approved transaction.
  name: authorizationCode
  type: string
- description: Amount appearing on the cardholder statement in the billing currency, without decimals.
  name: billingAmount
  type: string
- description: ISO 4217 numeric currency code for the billing amount.
  name: billingCurrency
  type: string
- description: Currency conversion rate applied when the transaction and billing currencies differ.
  name: conversionRate
  type: string
- description: Payment network through which the transaction was processed.
  name: network
  type: string
- description: The channel through which the payment was initiated.
  name: channel
  type: string
- description: Point of service entry mode indicating how the card data was captured at the terminal.
  name: posEntryMode
  type: string
- description: Unique code identifying a terminal at the card acceptor location.
  name: terminalId
  type: string
- description: Date on which the transaction settles, in YYYYMMDD format.
  name: settlementDate
  type: string
- description: External reference identifier provided by the originator for reconciliation.
  name: referenceId
  type: string
- description: Brief description or comment provided by the originator supporting the payment.
  name: memo
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/payment.json
slug: payment
source_filename: payment.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://github.com/api-evangelist/mastercard/blob/main/json-schema/payment.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Mastercard Payment\",\n  \"description\": \"A payment transaction processed through the Mastercard network, representing a transfer of funds between a payer and payee. Applicable across Mastercard Send, Account to Account Commerce, Bill Pay, and checkout solutions.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"paymentId\",\n    \"paymentType\",\n    \"amount\",\n    \"currency\",\n    \"status\"\n  ],\n  \"properties\": {\n    \"paymentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the payment, generated using UUID logic to unambiguously link request and response messages.\",\n      \"format\": \"uuid\",\n      \"examples\": [\"ecb2d942-eabd-42b6-87fd-69c19692bdc6\"]\n    },\n    \"paymentType\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"Classification of the payment indicating its purpose and processing path.\",\n      \"enum\": [\n        \"P2P\",\n        \"P2M\",\n        \"B2B\",\n        \"DISBURSEMENT\",\n        \"FUNDING\",\n        \"BILL_PAYMENT\",\n        \"ACCOUNT_TO_ACCOUNT\",\n        \"CARD_ON_FILE\",\n        \"RECURRING\",\n        \"REFUND\"\n      ]\n    },\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"Payment amount without decimal separators. The number of implied decimal places depends on the currency. For example, 10350 in USD represents $103.50.\",\n      \"pattern\": \"^[0-9]+$\",\n      \"minLength\": 1,\n      \"maxLength\": 12,\n      \"examples\": [\"10350\"]\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 numeric currency code for the payment amount.\",\n      \"pattern\": \"^[0-9]{3}$\",\n      \"minLength\": 3,\n      \"maxLength\": 3,\n      \"examples\": [\"840\"]\n    },\n    \"status\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"Current status of the payment in its lifecycle.\",\n      \"enum\": [\n        \"PENDING\",\n        \"AUTHORIZED\",\n        \"CAPTURED\",\n        \"SETTLED\",\n        \"DECLINED\",\n        \"CANCELLED\",\n        \"REFUNDED\",\n        \"FAILED\"\n      ]\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the payment initiation in ISO 8601 format with timezone offset.\",\n      \"format\": \"date-time\",\n      \"examples\": [\"2024-02-02T02:34:37-06:00\"]\n    },\n    \"sender\": {\n      \"$ref\": \"#/$defs/PaymentParty\",\n      \"description\": \"The party initiating or funding the payment.\"\n    },\n    \"recipient\": {\n      \"$ref\": \"#/$defs/PaymentParty\",\n      \"description\": \"The party receiving the payment funds.\"\n    },\n    \"cardNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Primary Account Number (PAN) of the card used for the payment. Must pass Luhn\
  \ algorithm validation.\",\n      \"pattern\": \"^[0-9]{12,19}$\",\n      \"minLength\": 12,\n      \"maxLength\": 19\n    },\n    \"tokenNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Payment token representing the card number for tokenized transactions (MDES).\",\n      \"pattern\": \"^[0-9]{12,19}$\",\n      \"minLength\": 12,\n      \"maxLength\": 19\n    },\n    \"merchantId\": {\n      \"type\": \"string\",\n      \"description\": \"Card acceptor or merchant unique identification number assigned by the acquirer.\",\n      \"maxLength\": 15,\n      \"examples\": [\"A42E51982100100\"]\n    },\n    \"merchantName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the card acceptor or merchant.\",\n      \"maxLength\": 22,\n      \"examples\": [\"ACME STORE\"]\n    },\n    \"merchantCategoryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Four-digit ISO 18245 Merchant Category Code (MCC) classifying the type of business.\",\n     \
  \ \"pattern\": \"^[0-9]{4}$\",\n      \"minLength\": 4,\n      \"maxLength\": 4,\n      \"examples\": [\"5411\"]\n    },\n    \"acquirerId\": {\n      \"type\": \"string\",\n      \"description\": \"Interbank Card Association (ICA) number of the acquiring institution.\",\n      \"minLength\": 3,\n      \"maxLength\": 7,\n      \"examples\": [\"5450\"]\n    },\n    \"icaNumber\": {\n      \"type\": \"string\",\n      \"description\": \"ICA number of the issuer or acquirer initiating the request.\",\n      \"minLength\": 3,\n      \"maxLength\": 7,\n      \"examples\": [\"1076\"]\n    },\n    \"authorizationCode\": {\n      \"type\": \"string\",\n      \"description\": \"Authorization code returned by the issuer for an approved transaction.\",\n      \"maxLength\": 6\n    },\n    \"billingAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Amount appearing on the cardholder statement in the billing currency, without decimals.\",\n      \"pattern\": \"^[0-9]+$\",\n      \"\
  minLength\": 1,\n      \"maxLength\": 12,\n      \"examples\": [\"10350\"]\n    },\n    \"billingCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 numeric currency code for the billing amount.\",\n      \"pattern\": \"^[0-9]{3}$\",\n      \"minLength\": 3,\n      \"maxLength\": 3,\n      \"examples\": [\"840\"]\n    },\n    \"conversionRate\": {\n      \"type\": \"string\",\n      \"description\": \"Currency conversion rate applied when the transaction and billing currencies differ.\"\n    },\n    \"network\": {\n      \"type\": \"string\",\n      \"description\": \"Payment network through which the transaction was processed.\",\n      \"enum\": [\n        \"MASTERCARD\",\n        \"MAESTRO\",\n        \"CIRRUS\"\n      ],\n      \"default\": \"MASTERCARD\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"The channel through which the payment was initiated.\",\n      \"enum\": [\n        \"POS\",\n        \"ECOMMERCE\",\n  \
  \      \"MOBILE\",\n        \"ATM\",\n        \"MOTO\",\n        \"RECURRING\",\n        \"IN_APP\"\n      ]\n    },\n    \"posEntryMode\": {\n      \"type\": \"string\",\n      \"description\": \"Point of service entry mode indicating how the card data was captured at the terminal.\",\n      \"maxLength\": 3,\n      \"examples\": [\"051\"]\n    },\n    \"terminalId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique code identifying a terminal at the card acceptor location.\",\n      \"maxLength\": 8,\n      \"examples\": [\"5055D305\"]\n    },\n    \"settlementDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date on which the transaction settles, in YYYYMMDD format.\",\n      \"pattern\": \"^[0-9]{8}$\",\n      \"examples\": [\"20240116\"]\n    },\n    \"referenceId\": {\n      \"type\": \"string\",\n      \"description\": \"External reference identifier provided by the originator for reconciliation.\",\n      \"maxLength\": 36\n    },\n    \"memo\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Brief description or comment provided by the originator supporting the payment.\",\n      \"maxLength\": 1000\n    }\n  },\n  \"$defs\": {\n    \"PaymentParty\": {\n      \"type\": \"object\",\n      \"description\": \"A party involved in a payment transaction, either as sender or recipient.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Full name of the payment party.\",\n          \"maxLength\": 100\n        },\n        \"accountNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Account number of the payment party.\",\n          \"maxLength\": 19\n        },\n        \"institutionId\": {\n          \"type\": \"string\",\n          \"description\": \"Identifier for the financial institution of the payment party.\",\n          \"maxLength\": 11\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/Address\"\n        }\n      }\n  \
  \  },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A postal address.\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\",\n          \"description\": \"First line of the street address.\",\n          \"maxLength\": 50\n        },\n        \"line2\": {\n          \"type\": \"string\",\n          \"description\": \"Second line of the street address.\",\n          \"maxLength\": 50\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City name.\",\n          \"maxLength\": 50\n        },\n        \"stateProvinceCode\": {\n          \"type\": \"string\",\n          \"description\": \"State or province code.\",\n          \"maxLength\": 3\n        },\n        \"postalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code.\",\n          \"maxLength\": 10\n        },\n        \"countryCode\": {\n          \"type\": \"string\",\n          \"description\":\
  \ \"ISO 3166-1 alpha-3 country code.\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"minLength\": 3,\n          \"maxLength\": 3\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/payment.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Mastercard Payment
---
