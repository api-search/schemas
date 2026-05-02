---
description: Schema for a Moov money movement transfer between two accounts. Transfers move funds via ACH, RTP, or card rails and have a source payment method and a destination payment method. The transfer progresses through a lifecycle from created to completed or failed.
layout: schema
name: Moov Transfer
properties_list:
- description: Unique identifier for the transfer assigned by Moov.
  name: transferID
  type: string
- description: Current lifecycle status of the transfer.
  name: status
  type: string
- description: The payment method and account from which funds are debited.
  name: source
  type: object
- description: The payment method and account to which funds are credited.
  name: destination
  type: object
- description: The total amount being transferred.
  name: amount
  type: object
- description: Human-readable description of the transfer purpose.
  name: description
  type: string
- description: Custom key-value pairs for application-specific data attached to the transfer.
  name: metadata
  type: object
- description: Optional fee amount collected by the platform facilitator on this transfer.
  name: facilitatorFee
  type: object
- description: Moov platform fee in cents charged for processing the transfer.
  name: moovFee
  type: integer
- description: Moov platform fee expressed as a decimal string for high-precision representation.
  name: moovFeeDecimal
  type: string
- description: ISO 8601 timestamp when the transfer was created.
  name: createdOn
  type: string
- description: ISO 8601 timestamp when the transfer was last updated.
  name: updatedOn
  type: string
- description: ISO 8601 timestamp when the transfer reached a terminal status.
  name: completedOn
  type: string
provider_name: Moov
provider_slug: moov
schema_file: json-schema/moov-transfer-schema.json
slug: moov-transfer
source_filename: moov-transfer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.moov.io/schemas/moov/transfer.json\",\n  \"title\": \"Moov Transfer\",\n  \"description\": \"Schema for a Moov money movement transfer between two accounts. Transfers move funds via ACH, RTP, or card rails and have a source payment method and a destination payment method. The transfer progresses through a lifecycle from created to completed or failed.\",\n  \"type\": \"object\",\n  \"required\": [\"transferID\", \"status\", \"source\", \"destination\", \"amount\", \"createdOn\"],\n  \"properties\": {\n    \"transferID\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the transfer assigned by Moov.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the transfer.\",\n      \"enum\": [\"created\", \"pending\", \"completed\", \"failed\", \"reversed\"]\n    },\n    \"\
  source\": {\n      \"$ref\": \"#/$defs/TransferParticipant\",\n      \"description\": \"The payment method and account from which funds are debited.\"\n    },\n    \"destination\": {\n      \"$ref\": \"#/$defs/TransferParticipant\",\n      \"description\": \"The payment method and account to which funds are credited.\"\n    },\n    \"amount\": {\n      \"$ref\": \"#/$defs/Amount\",\n      \"description\": \"The total amount being transferred.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the transfer purpose.\",\n      \"maxLength\": 100\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom key-value pairs for application-specific data attached to the transfer.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"facilitatorFee\": {\n      \"$ref\": \"#/$defs/Amount\",\n      \"description\": \"Optional fee amount collected by the platform\
  \ facilitator on this transfer.\"\n    },\n    \"moovFee\": {\n      \"type\": \"integer\",\n      \"description\": \"Moov platform fee in cents charged for processing the transfer.\",\n      \"minimum\": 0\n    },\n    \"moovFeeDecimal\": {\n      \"type\": \"string\",\n      \"description\": \"Moov platform fee expressed as a decimal string for high-precision representation.\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d+$\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the transfer was created.\"\n    },\n    \"updatedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the transfer was last updated.\"\n    },\n    \"completedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the transfer reached a terminal status.\"\n    }\n  },\n  \"$defs\": {\n    \"Amount\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"A monetary amount with ISO 4217 currency denomination.\",\n      \"required\": [\"currency\", \"value\"],\n      \"properties\": {\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 three-letter currency code (e.g., USD).\",\n          \"minLength\": 3,\n          \"maxLength\": 3,\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"value\": {\n          \"type\": \"integer\",\n          \"description\": \"Amount in the smallest currency unit (e.g., cents for USD). Must be a non-negative integer.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"TransferParticipant\": {\n      \"type\": \"object\",\n      \"description\": \"One side of a transfer, representing the payment method and account involved.\",\n      \"required\": [\"paymentMethodID\"],\n      \"properties\": {\n        \"paymentMethodID\": {\n          \"type\": \"string\",\n          \"format\": \"\
  uuid\",\n          \"description\": \"Unique identifier of the payment method used for this side of the transfer.\"\n        },\n        \"paymentMethodType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of payment instrument used.\",\n          \"enum\": [\n            \"moov-wallet\",\n            \"ach-debit-fund\",\n            \"ach-debit-collect\",\n            \"ach-credit-standard\",\n            \"ach-credit-same-day\",\n            \"rtp-credit\",\n            \"card-payment\"\n          ]\n        },\n        \"account\": {\n          \"$ref\": \"#/$defs/AccountRef\",\n          \"description\": \"Reference to the Moov account on this side of the transfer.\"\n        },\n        \"bankAccount\": {\n          \"$ref\": \"#/$defs/BankAccountRef\",\n          \"description\": \"Bank account details when the payment method type is an ACH rail.\"\n        },\n        \"wallet\": {\n          \"$ref\": \"#/$defs/WalletRef\",\n          \"description\"\
  : \"Wallet details when the payment method type is moov-wallet.\"\n        },\n        \"card\": {\n          \"$ref\": \"#/$defs/CardRef\",\n          \"description\": \"Card details when the payment method type is card-payment.\"\n        }\n      }\n    },\n    \"AccountRef\": {\n      \"type\": \"object\",\n      \"description\": \"A lightweight reference to a Moov account.\",\n      \"properties\": {\n        \"accountID\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the Moov account.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address of the account holder.\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the account.\"\n        }\n      }\n    },\n    \"BankAccountRef\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of a\
  \ linked bank account involved in a transfer.\",\n      \"properties\": {\n        \"bankAccountID\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the bank account.\"\n        },\n        \"bankName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the financial institution.\"\n        },\n        \"bankAccountType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of bank account.\",\n          \"enum\": [\"checking\", \"savings\", \"loan\"]\n        },\n        \"lastFourAccountNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Last four digits of the bank account number for identification.\",\n          \"pattern\": \"^\\\\d{4}$\"\n        },\n        \"routingNumber\": {\n          \"type\": \"string\",\n          \"description\": \"ABA routing transit number for the bank.\",\n          \"pattern\": \"^\\\\d{9}$\"\n        }\n      }\n \
  \   },\n    \"WalletRef\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a Moov digital wallet involved in a transfer.\",\n      \"properties\": {\n        \"walletID\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the wallet.\"\n        }\n      }\n    },\n    \"CardRef\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of a linked card involved in a transfer.\",\n      \"properties\": {\n        \"cardID\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the card.\"\n        },\n        \"brand\": {\n          \"type\": \"string\",\n          \"description\": \"Card network brand.\",\n          \"enum\": [\"Visa\", \"Mastercard\", \"AmericanExpress\", \"Discover\", \"DinersClub\", \"JCB\"]\n        },\n        \"cardType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of card\
  \ instrument.\",\n          \"enum\": [\"debit\", \"credit\", \"prepaid\", \"unknown\"]\n        },\n        \"lastFourCardNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Last four digits of the card number.\",\n          \"pattern\": \"^\\\\d{4}$\"\n        },\n        \"expiration\": {\n          \"type\": \"object\",\n          \"description\": \"Card expiration date.\",\n          \"properties\": {\n            \"month\": {\n              \"type\": \"string\",\n              \"description\": \"Two-digit expiration month.\",\n              \"pattern\": \"^(0[1-9]|1[0-2])$\"\n            },\n            \"year\": {\n              \"type\": \"string\",\n              \"description\": \"Two-digit expiration year.\",\n              \"pattern\": \"^\\\\d{2}$\"\n            }\n          }\n        }\n      }\n    },\n    \"Refund\": {\n      \"type\": \"object\",\n      \"description\": \"A refund issued against a completed card transfer, returning funds to the\
  \ original payment method.\",\n      \"required\": [\"refundID\", \"status\", \"amount\"],\n      \"properties\": {\n        \"refundID\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the refund.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current processing status of the refund.\",\n          \"enum\": [\"created\", \"pending\", \"completed\", \"failed\"]\n        },\n        \"amount\": {\n          \"$ref\": \"#/$defs/Amount\",\n          \"description\": \"Amount being refunded. Must not exceed the original transfer amount.\"\n        },\n        \"createdOn\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the refund was initiated.\"\n        },\n        \"updatedOn\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO\
  \ 8601 timestamp when the refund was last updated.\"\n        }\n      }\n    },\n    \"TransferCancellation\": {\n      \"type\": \"object\",\n      \"description\": \"A cancellation request for a pending transfer that has not yet been submitted to the payment rail.\",\n      \"required\": [\"cancellationID\", \"status\"],\n      \"properties\": {\n        \"cancellationID\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the cancellation request.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Status of the cancellation request.\",\n          \"enum\": [\"pending\", \"confirmed\", \"declined\"]\n        },\n        \"createdOn\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the cancellation was requested.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moov/refs/heads/main/json-schema/moov-transfer-schema.json
tags:
- Banking
- Embedded Finance
- Financial Infrastructure
- Money Movement
- Payments
- Transfers
title: Moov Transfer
---
