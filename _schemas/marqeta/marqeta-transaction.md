---
description: A Marqeta transaction record representing a card payment event such as an authorization, clearing, decline, GPA debit, GPA credit, or refund. Transactions are created by the Marqeta platform in response to card network messages and are associated with a specific card, cardholder, and card acceptor.
layout: schema
name: Marqeta Transaction
properties_list:
- description: Unique identifier for the transaction on the Marqeta platform.
  name: token
  type: string
- description: Transaction type describing the nature of the event. Common values include authorization, authorization.clearing, authorization.advice, pindebit, refund, gpa.credit, gpa.debit, and transfer.
  name: type
  type: string
- description: Current lifecycle state of the transaction.
  name: state
  type: string
- description: Unique identifier assigned by the card network for the transaction.
  name: identifier
  type: string
- description: Token of the cardholder (user) associated with this transaction.
  name: user_token
  type: string
- description: Token of the business account holder associated with this transaction, if applicable.
  name: business_token
  type: string
- description: Token of the payment card used in this transaction.
  name: card_token
  type: string
- description: Token of the card product associated with the card used.
  name: card_product_token
  type: string
- description: Transaction amount in the cardholder billing currency.
  name: amount
  type: number
- description: ISO 4217 three-letter currency code for the transaction amount.
  name: currency_code
  type: string
- description: Original transaction amount in the merchant transaction currency, before any currency conversion.
  name: orig_amount
  type: number
- description: ISO 4217 currency code for the original transaction currency at the merchant.
  name: orig_currency_code
  type: string
- description: ''
  name: card_acceptor
  type: object
- description: ''
  name: response
  type: object
- description: ''
  name: gpa
  type: object
- description: GPA order details if this transaction is associated with a fund load.
  name: gpa_order
  type: object
- description: List of fees applied to this transaction.
  name: fees
  type: array
- description: ''
  name: pos
  type: object
- description: Card network that processed the transaction.
  name: network
  type: string
- description: Fee amount charged by the acquirer for this transaction.
  name: acquirer_fee_amount
  type: number
- description: Acquirer information for the transaction.
  name: acquirer
  type: object
- description: Tokens of related transactions, such as the original authorization for a clearing event.
  name: related_transactions
  type: array
- description: ISO 8601 timestamp when the transaction was created on the Marqeta platform.
  name: created_time
  type: string
- description: ISO 8601 timestamp of the transaction as reported by the card network.
  name: user_transaction_time
  type: string
- description: Date on which the transaction settled with the card network.
  name: settlement_date
  type: string
provider_name: marqeta
provider_slug: marqeta
schema_file: json-schema/marqeta-transaction-schema.json
slug: marqeta-transaction
source_filename: marqeta-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://marqeta.com/schemas/transaction.json\",\n  \"title\": \"Marqeta Transaction\",\n  \"description\": \"A Marqeta transaction record representing a card payment event such as an authorization, clearing, decline, GPA debit, GPA credit, or refund. Transactions are created by the Marqeta platform in response to card network messages and are associated with a specific card, cardholder, and card acceptor.\",\n  \"type\": \"object\",\n  \"required\": [\"token\", \"type\", \"state\", \"created_time\"],\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the transaction on the Marqeta platform.\",\n      \"maxLength\": 36\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction type describing the nature of the event. Common values include authorization, authorization.clearing, authorization.advice,\
  \ pindebit, refund, gpa.credit, gpa.debit, and transfer.\",\n      \"examples\": [\n        \"authorization\",\n        \"authorization.clearing\",\n        \"authorization.advice\",\n        \"pindebit\",\n        \"refund\",\n        \"gpa.credit\",\n        \"gpa.debit\",\n        \"transfer\"\n      ]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle state of the transaction.\",\n      \"enum\": [\"PENDING\", \"COMPLETION\", \"DECLINED\", \"ERROR\", \"ALL\", \"VOID\"]\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned by the card network for the transaction.\",\n      \"maxLength\": 255\n    },\n    \"user_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token of the cardholder (user) associated with this transaction.\",\n      \"maxLength\": 36\n    },\n    \"business_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token of the business\
  \ account holder associated with this transaction, if applicable.\",\n      \"maxLength\": 36\n    },\n    \"card_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token of the payment card used in this transaction.\",\n      \"maxLength\": 36\n    },\n    \"card_product_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token of the card product associated with the card used.\",\n      \"maxLength\": 36\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Transaction amount in the cardholder billing currency.\",\n      \"minimum\": 0\n    },\n    \"currency_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 three-letter currency code for the transaction amount.\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"orig_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Original transaction amount in the merchant transaction currency, before any currency conversion.\",\n      \"minimum\":\
  \ 0\n    },\n    \"orig_currency_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the original transaction currency at the merchant.\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"card_acceptor\": {\n      \"$ref\": \"#/$defs/CardAcceptor\"\n    },\n    \"response\": {\n      \"$ref\": \"#/$defs/TransactionResponse\"\n    },\n    \"gpa\": {\n      \"$ref\": \"#/$defs/GpaBalance\"\n    },\n    \"gpa_order\": {\n      \"type\": \"object\",\n      \"description\": \"GPA order details if this transaction is associated with a fund load.\",\n      \"properties\": {\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"Token of the GPA order.\"\n        },\n        \"funding_source_token\": {\n          \"type\": \"string\",\n          \"description\": \"Token of the funding source used for the GPA order.\"\n        }\n      }\n    },\n    \"fees\": {\n      \"type\": \"array\",\n      \"description\": \"List of fees\
  \ applied to this transaction.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/FeeDetail\"\n      }\n    },\n    \"pos\": {\n      \"$ref\": \"#/$defs/PosData\"\n    },\n    \"network\": {\n      \"type\": \"string\",\n      \"description\": \"Card network that processed the transaction.\",\n      \"enum\": [\"VISA\", \"MASTERCARD\", \"PULSE\", \"STAR\", \"ACCEL\", \"NY_SWITCH\", \"CU24\"]\n    },\n    \"acquirer_fee_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Fee amount charged by the acquirer for this transaction.\"\n    },\n    \"acquirer\": {\n      \"type\": \"object\",\n      \"description\": \"Acquirer information for the transaction.\",\n      \"properties\": {\n        \"institution_country\": {\n          \"type\": \"string\",\n          \"description\": \"Country of the acquiring institution.\"\n        },\n        \"institution_id_code\": {\n          \"type\": \"string\",\n          \"description\": \"Acquiring institution identifier code.\"\n  \
  \      },\n        \"retrieval_reference_number\": {\n          \"type\": \"string\",\n          \"description\": \"Retrieval reference number assigned by the acquirer.\"\n        }\n      }\n    },\n    \"related_transactions\": {\n      \"type\": \"array\",\n      \"description\": \"Tokens of related transactions, such as the original authorization for a clearing event.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"related_transaction_token\": {\n            \"type\": \"string\",\n            \"description\": \"Token of the related transaction.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Relationship type (e.g., ORIGINAL_AUTHORIZATION).\"\n          }\n        }\n      }\n    },\n    \"created_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the transaction was created on the Marqeta platform.\"\n    },\n\
  \    \"user_transaction_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the transaction as reported by the card network.\"\n    },\n    \"settlement_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date on which the transaction settled with the card network.\"\n    }\n  },\n  \"$defs\": {\n    \"CardAcceptor\": {\n      \"type\": \"object\",\n      \"description\": \"Merchant or card acceptor information for the transaction.\",\n      \"properties\": {\n        \"mid\": {\n          \"type\": \"string\",\n          \"description\": \"Merchant identifier assigned by the card network.\",\n          \"maxLength\": 15\n        },\n        \"mcc\": {\n          \"type\": \"string\",\n          \"description\": \"Merchant category code identifying the type of business.\",\n          \"pattern\": \"^\\\\d{4}$\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"Name of the merchant or card acceptor.\",\n          \"maxLength\": 25\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Street address of the merchant location.\",\n          \"maxLength\": 25\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City of the merchant location.\",\n          \"maxLength\": 13\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"State or province of the merchant location.\",\n          \"maxLength\": 3\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"description\": \"ZIP or postal code of the merchant location.\",\n          \"maxLength\": 10\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 3166-1 alpha-3 country code of the merchant.\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"poi\": {\n\
  \          \"$ref\": \"#/$defs/PointOfInteraction\"\n        }\n      }\n    },\n    \"PointOfInteraction\": {\n      \"type\": \"object\",\n      \"description\": \"Point of interaction data describing how the card was presented.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Terminal type at the point of interaction.\",\n          \"enum\": [\"ATM\", \"AUTOFUEL_DISPENSERS\", \"CASH_REGISTER\", \"ECOMMERCE\", \"MOTO\", \"POS\", \"RECURRING_PAYMENTS\", \"UNATTENDED_PAYMENT_TERMINAL\"]\n        },\n        \"partial_approval_capable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the terminal supports partial approvals.\"\n        },\n        \"installment_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of installment payment if applicable.\"\n        }\n      }\n    },\n    \"TransactionResponse\": {\n      \"type\": \"object\",\n      \"description\": \"Authorization\
  \ response from the Marqeta platform or card network.\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Response code. 00 indicates approval. Other values indicate decline reasons.\",\n          \"pattern\": \"^\\\\d{2,4}$\"\n        },\n        \"memo\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable response message describing the authorization result.\",\n          \"maxLength\": 255\n        }\n      }\n    },\n    \"GpaBalance\": {\n      \"type\": \"object\",\n      \"description\": \"General purpose account (GPA) balance state after a transaction.\",\n      \"properties\": {\n        \"currency_code\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 currency code for the GPA balance.\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"ledger_balance\": {\n          \"type\": \"number\",\n          \"description\": \"Total ledger balance including\
  \ all pending transactions.\"\n        },\n        \"available_balance\": {\n          \"type\": \"number\",\n          \"description\": \"Available balance that can be spent immediately.\"\n        },\n        \"credit_balance\": {\n          \"type\": \"number\",\n          \"description\": \"Credit balance applied to the account.\"\n        },\n        \"pending_credits\": {\n          \"type\": \"number\",\n          \"description\": \"Pending credits not yet settled into the available balance.\"\n        },\n        \"impacted_amount\": {\n          \"type\": \"number\",\n          \"description\": \"Balance amount affected by the current transaction.\"\n        }\n      }\n    },\n    \"FeeDetail\": {\n      \"type\": \"object\",\n      \"description\": \"Detail of a fee applied to a transaction.\",\n      \"properties\": {\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the fee record.\"\n        },\n        \"fee_token\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Token of the fee configuration that was applied.\"\n        },\n        \"amount\": {\n          \"type\": \"number\",\n          \"description\": \"Fee amount charged.\",\n          \"minimum\": 0\n        },\n        \"memo\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the fee.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Fee type identifier.\"\n        }\n      }\n    },\n    \"PosData\": {\n      \"type\": \"object\",\n      \"description\": \"Point-of-sale terminal data from the card network message.\",\n      \"properties\": {\n        \"terminal_attendance\": {\n          \"type\": \"string\",\n          \"description\": \"Whether terminal is attended by a merchant employee.\",\n          \"enum\": [\"ATTENDED\", \"UNATTENDED\", \"NONE\"]\n        },\n        \"terminal_location\": {\n          \"type\": \"string\",\n      \
  \    \"description\": \"Physical location type of the terminal.\",\n          \"enum\": [\"ON_PREMISE\", \"OFF_PREMISE\", \"NONE\"]\n        },\n        \"cardholder_presence\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the cardholder was present at the terminal.\",\n          \"enum\": [\"PRESENT\", \"NOT_PRESENT\", \"MAIL_ORDER\", \"PHONE_ORDER\", \"STANDING_ORDER\", \"ELECTRONIC_ORDER\", \"NOT_PRESENT_RECURRING\"]\n        },\n        \"card_presence\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the physical card was present.\",\n          \"enum\": [\"PRESENT\", \"NOT_PRESENT\"]\n        },\n        \"card_data_input_capability\": {\n          \"type\": \"string\",\n          \"description\": \"Method by which card data was read.\",\n          \"enum\": [\"UNKNOWN\", \"NO_TERMINAL\", \"MAGNETIC_STRIPE\", \"BARCODE\", \"OCR\", \"CHIP_AND_PIN\", \"CONTACTLESS\", \"CONTACTLESS_AND_MAGNETIC_STRIPE\", \"CREDENTIAL_ON_FILE\", \"\
  MANUAL\", \"MANUAL_AND_CHIP\"]\n        },\n        \"pin_entry_mode\": {\n          \"type\": \"string\",\n          \"description\": \"Whether PIN entry was required and performed.\",\n          \"enum\": [\"TRUE\", \"FALSE\", \"CREDENTIAL_ON_FILE\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/json-schema/marqeta-transaction-schema.json
tags: []
title: Marqeta Transaction
---
