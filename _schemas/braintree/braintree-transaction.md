---
description: Represents a payment transaction processed through the Braintree gateway. A transaction captures the full lifecycle from authorization through settlement, refund, or void, and supports credit and debit cards, PayPal, Apple Pay, Google Pay, Venmo, ACH, and SEPA payment methods.
layout: schema
name: Braintree Transaction
properties_list:
- description: Unique identifier for the transaction assigned by Braintree.
  name: id
  type: string
- description: The transaction amount as a decimal string in the transaction currency.
  name: amount
  type: string
- description: The current processing status of the transaction.
  name: status
  type: string
- description: The type of transaction. 'sale' represents a charge and 'credit' represents a refund.
  name: type
  type: string
- description: ISO 4217 three-letter currency code for the transaction.
  name: currency_iso_code
  type: string
- description: Merchant-provided order identifier associated with this transaction for reconciliation.
  name: order_id
  type: string
- description: Identifier of the Braintree merchant account used to process this transaction.
  name: merchant_account_id
  type: string
- description: Identifier of the customer in the Braintree Vault associated with this transaction, if applicable.
  name: customer_id
  type: string
- description: Token of the vaulted payment method used for this transaction, if applicable.
  name: payment_method_token
  type: string
- description: The one-time payment method nonce used for this transaction, if applicable.
  name: payment_method_nonce
  type: string
- description: The processor-specific response code returned when the transaction was processed.
  name: processor_response_code
  type: string
- description: Human-readable text description of the processor response code.
  name: processor_response_text
  type: string
- description: The reason the Braintree gateway rejected the transaction, if applicable.
  name: gateway_rejection_reason
  type: string
- description: The tax amount included in the transaction total, as a decimal string.
  name: tax_amount
  type: string
- description: The shipping amount included in the transaction total, as a decimal string.
  name: shipping_amount
  type: string
- description: Indicates the origin of the transaction for network reporting requirements.
  name: transaction_source
  type: string
- description: Billing address associated with this transaction.
  name: billing
  type: object
- description: Shipping address associated with this transaction.
  name: shipping
  type: object
- description: Summary of the customer associated with this transaction.
  name: customer_details
  type: object
- description: Masked credit or debit card details used in this transaction.
  name: credit_card_details
  type: object
- description: Dynamic descriptor fields that appear on the customer's bank statement.
  name: descriptor
  type: object
- description: List of transaction identifiers for refund transactions created against this transaction.
  name: refund_ids
  type: array
- description: For refund transactions, the identifier of the original transaction being refunded.
  name: refunded_transaction_id
  type: string
- description: Identifier of the subscription that generated this transaction, if applicable.
  name: subscription_id
  type: string
- description: Line items for Level 3 processing data, up to 249 items.
  name: line_items
  type: array
- description: Disbursement information for when the transaction funds were or will be sent to the merchant.
  name: disbursement_details
  type: object
- description: Timestamp when the transaction was created, in ISO 8601 format.
  name: created_at
  type: string
- description: Timestamp when the transaction was last updated, in ISO 8601 format.
  name: updated_at
  type: string
provider_name: braintree
provider_slug: braintree
schema_file: json-schema/braintree-transaction-schema.json
slug: braintree-transaction
source_filename: braintree-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/braintree/schemas/transaction.json\",\n  \"title\": \"Braintree Transaction\",\n  \"description\": \"Represents a payment transaction processed through the Braintree gateway. A transaction captures the full lifecycle from authorization through settlement, refund, or void, and supports credit and debit cards, PayPal, Apple Pay, Google Pay, Venmo, ACH, and SEPA payment methods.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"amount\", \"status\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the transaction assigned by Braintree.\",\n      \"minLength\": 1\n    },\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"The transaction amount as a decimal string in the transaction currency.\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d{2}$\",\n      \"example\": \"\
  10.00\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current processing status of the transaction.\",\n      \"enum\": [\n        \"authorization_expired\",\n        \"authorized\",\n        \"authorizing\",\n        \"settlement_confirmed\",\n        \"settlement_declined\",\n        \"settlement_pending\",\n        \"settled\",\n        \"settling\",\n        \"submitted_for_settlement\",\n        \"voided\",\n        \"processor_declined\",\n        \"failed\",\n        \"gateway_rejected\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of transaction. 'sale' represents a charge and 'credit' represents a refund.\",\n      \"enum\": [\"sale\", \"credit\"]\n    },\n    \"currency_iso_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 three-letter currency code for the transaction.\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"example\": \"USD\"\n    },\n    \"order_id\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Merchant-provided order identifier associated with this transaction for reconciliation.\",\n      \"maxLength\": 255\n    },\n    \"merchant_account_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the Braintree merchant account used to process this transaction.\"\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the customer in the Braintree Vault associated with this transaction, if applicable.\",\n      \"maxLength\": 36\n    },\n    \"payment_method_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token of the vaulted payment method used for this transaction, if applicable.\"\n    },\n    \"payment_method_nonce\": {\n      \"type\": \"string\",\n      \"description\": \"The one-time payment method nonce used for this transaction, if applicable.\"\n    },\n    \"processor_response_code\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The processor-specific response code returned when the transaction was processed.\",\n      \"pattern\": \"^\\\\d{4}$\"\n    },\n    \"processor_response_text\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable text description of the processor response code.\"\n    },\n    \"gateway_rejection_reason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the Braintree gateway rejected the transaction, if applicable.\",\n      \"enum\": [\n        \"avs\",\n        \"avs_and_cvv\",\n        \"cvv\",\n        \"duplicate\",\n        \"fraud\",\n        \"risk_threshold\",\n        \"three_d_secure\",\n        \"token_issuance\",\n        \"application_incomplete\"\n      ]\n    },\n    \"tax_amount\": {\n      \"type\": \"string\",\n      \"description\": \"The tax amount included in the transaction total, as a decimal string.\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d{2}$\"\n    },\n    \"shipping_amount\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"The shipping amount included in the transaction total, as a decimal string.\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d{2}$\"\n    },\n    \"transaction_source\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the origin of the transaction for network reporting requirements.\",\n      \"enum\": [\"recurring\", \"recurring_first\", \"unscheduled\", \"moto\"]\n    },\n    \"billing\": {\n      \"$ref\": \"#/$defs/Address\",\n      \"description\": \"Billing address associated with this transaction.\"\n    },\n    \"shipping\": {\n      \"$ref\": \"#/$defs/Address\",\n      \"description\": \"Shipping address associated with this transaction.\"\n    },\n    \"customer_details\": {\n      \"$ref\": \"#/$defs/CustomerSummary\",\n      \"description\": \"Summary of the customer associated with this transaction.\"\n    },\n    \"credit_card_details\": {\n      \"$ref\": \"#/$defs/CreditCardDetails\",\n      \"description\": \"Masked credit or debit card\
  \ details used in this transaction.\"\n    },\n    \"descriptor\": {\n      \"$ref\": \"#/$defs/Descriptor\",\n      \"description\": \"Dynamic descriptor fields that appear on the customer's bank statement.\"\n    },\n    \"refund_ids\": {\n      \"type\": \"array\",\n      \"description\": \"List of transaction identifiers for refund transactions created against this transaction.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"Unique identifier of a refund transaction.\"\n      }\n    },\n    \"refunded_transaction_id\": {\n      \"type\": \"string\",\n      \"description\": \"For refund transactions, the identifier of the original transaction being refunded.\"\n    },\n    \"subscription_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the subscription that generated this transaction, if applicable.\"\n    },\n    \"line_items\": {\n      \"type\": \"array\",\n      \"description\": \"Line items for Level 3 processing data,\
  \ up to 249 items.\",\n      \"maxItems\": 249,\n      \"items\": {\n        \"$ref\": \"#/$defs/LineItem\"\n      }\n    },\n    \"disbursement_details\": {\n      \"$ref\": \"#/$defs/DisbursementDetails\",\n      \"description\": \"Disbursement information for when the transaction funds were or will be sent to the merchant.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the transaction was created, in ISO 8601 format.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the transaction was last updated, in ISO 8601 format.\"\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A billing or shipping address associated with a transaction or customer.\",\n      \"properties\": {\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\":\
  \ \"First name of the address holder.\",\n          \"maxLength\": 255\n        },\n        \"last_name\": {\n          \"type\": \"string\",\n          \"description\": \"Last name of the address holder.\",\n          \"maxLength\": 255\n        },\n        \"company\": {\n          \"type\": \"string\",\n          \"description\": \"Company or organization name at this address.\",\n          \"maxLength\": 255\n        },\n        \"street_address\": {\n          \"type\": \"string\",\n          \"description\": \"Primary street address line.\",\n          \"maxLength\": 255\n        },\n        \"extended_address\": {\n          \"type\": \"string\",\n          \"description\": \"Secondary address line such as apartment or suite number.\",\n          \"maxLength\": 255\n        },\n        \"locality\": {\n          \"type\": \"string\",\n          \"description\": \"City or locality of the address.\",\n          \"maxLength\": 255\n        },\n        \"region\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"State, province, or region code of the address.\",\n          \"maxLength\": 255\n        },\n        \"postal_code\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code of the address.\",\n          \"maxLength\": 9\n        },\n        \"country_code_alpha2\": {\n          \"type\": \"string\",\n          \"description\": \"Two-letter ISO 3166-1 alpha-2 country code.\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"country_name\": {\n          \"type\": \"string\",\n          \"description\": \"Full country name.\",\n          \"maxLength\": 255\n        }\n      }\n    },\n    \"CustomerSummary\": {\n      \"type\": \"object\",\n      \"description\": \"A summary of the customer associated with a transaction.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the customer in the Braintree Vault.\",\n          \"\
  maxLength\": 36\n        },\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\": \"Customer's first name.\",\n          \"maxLength\": 255\n        },\n        \"last_name\": {\n          \"type\": \"string\",\n          \"description\": \"Customer's last name.\",\n          \"maxLength\": 255\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Customer's email address.\",\n          \"maxLength\": 255\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Customer's phone number.\",\n          \"maxLength\": 255\n        },\n        \"company\": {\n          \"type\": \"string\",\n          \"description\": \"Customer's company or organization name.\",\n          \"maxLength\": 255\n        }\n      }\n    },\n    \"CreditCardDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Masked credit or debit card details used\
  \ in a transaction.\",\n      \"properties\": {\n        \"bin\": {\n          \"type\": \"string\",\n          \"description\": \"First six digits of the card number, identifying the issuing bank and card type.\",\n          \"pattern\": \"^\\\\d{6}$\"\n        },\n        \"last_4\": {\n          \"type\": \"string\",\n          \"description\": \"Last four digits of the card number.\",\n          \"pattern\": \"^\\\\d{4}$\"\n        },\n        \"card_type\": {\n          \"type\": \"string\",\n          \"description\": \"The card network or brand.\",\n          \"enum\": [\n            \"American Express\",\n            \"Carte Blanche\",\n            \"China UnionPay\",\n            \"Diners Club\",\n            \"Discover\",\n            \"Elo\",\n            \"JCB\",\n            \"Laser\",\n            \"Maestro\",\n            \"MasterCard\",\n            \"Solo\",\n            \"Switch\",\n            \"Visa\",\n            \"Unknown\"\n          ]\n        },\n        \"expiration_month\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Two-digit expiration month of the card.\",\n          \"pattern\": \"^(0[1-9]|1[0-2])$\"\n        },\n        \"expiration_year\": {\n          \"type\": \"string\",\n          \"description\": \"Four-digit expiration year of the card.\",\n          \"pattern\": \"^\\\\d{4}$\"\n        },\n        \"cardholder_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the cardholder as it appears on the card.\",\n          \"maxLength\": 175\n        },\n        \"country_of_issuance\": {\n          \"type\": \"string\",\n          \"description\": \"Two-letter ISO 3166-1 country code of the card-issuing country.\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"Vault token for this card if it was stored during the transaction.\"\n        }\n      }\n    },\n    \"Descriptor\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Dynamic descriptor fields that appear on the cardholder's bank or credit card statement.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Merchant name as it appears on the customer's statement. Maximum 22 characters.\",\n          \"maxLength\": 22\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Merchant phone number as it appears on the customer's statement. 10–14 digits.\",\n          \"maxLength\": 14,\n          \"pattern\": \"^\\\\d{10,14}$\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"Merchant URL as it appears on the customer's statement. Maximum 13 characters.\",\n          \"maxLength\": 13\n        }\n      }\n    },\n    \"LineItem\": {\n      \"type\": \"object\",\n      \"description\": \"A single product or service line item included for Level 3 processing data.\",\n      \"required\"\
  : [\"name\", \"quantity\", \"unit_amount\", \"total_amount\", \"kind\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name or description of the product or service.\",\n          \"maxLength\": 127\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Additional description of the line item.\",\n          \"maxLength\": 127\n        },\n        \"kind\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this item is a debit (charge) or credit (discount/refund).\",\n          \"enum\": [\"debit\", \"credit\"]\n        },\n        \"quantity\": {\n          \"type\": \"string\",\n          \"description\": \"Quantity of the line item as a decimal string.\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d{4}$\",\n          \"example\": \"1.0000\"\n        },\n        \"unit_amount\": {\n          \"type\": \"string\",\n          \"description\": \"Unit price\
  \ of the line item as a decimal string.\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d{2}$\",\n          \"example\": \"5.00\"\n        },\n        \"total_amount\": {\n          \"type\": \"string\",\n          \"description\": \"Total amount for this line item (quantity × unit_amount) as a decimal string.\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d{2}$\",\n          \"example\": \"5.00\"\n        },\n        \"unit_of_measure\": {\n          \"type\": \"string\",\n          \"description\": \"Unit of measure for the quantity, such as 'each', 'kg', or 'oz'.\",\n          \"maxLength\": 12\n        },\n        \"commodity_code\": {\n          \"type\": \"string\",\n          \"description\": \"Commodity code identifying the type of goods for Level 3 processing.\",\n          \"maxLength\": 12\n        },\n        \"tax_amount\": {\n          \"type\": \"string\",\n          \"description\": \"Tax amount for this line item as a decimal string.\",\n          \"pattern\": \"^\\\\d+\\\\\
  .\\\\d{2}$\"\n        },\n        \"discount_amount\": {\n          \"type\": \"string\",\n          \"description\": \"Discount amount applied to this line item as a decimal string.\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d{2}$\"\n        },\n        \"product_code\": {\n          \"type\": \"string\",\n          \"description\": \"Merchant-defined product code or SKU for this line item.\",\n          \"maxLength\": 12\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the product page of this line item.\"\n        }\n      }\n    },\n    \"DisbursementDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Details about the disbursement of transaction funds to the merchant's bank account.\",\n      \"properties\": {\n        \"disbursement_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date on which the funds were or will be disbursed\
  \ to the merchant.\"\n        },\n        \"settlement_amount\": {\n          \"type\": \"string\",\n          \"description\": \"Amount that was or will be disbursed, in the settlement currency.\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d{2}$\"\n        },\n        \"settlement_currency_iso_code\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 currency code of the settlement currency.\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"funds_held\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, the funds are being held and not yet disbursed to the merchant.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/json-schema/braintree-transaction-schema.json
tags: []
title: Braintree Transaction
---
