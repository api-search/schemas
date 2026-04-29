---
description: Represents an Affirm payment transaction, capturing the full lifecycle from authorization through capture, refund, and void. Transactions are created by exchanging a checkout token via the Transactions API after a customer completes the Affirm checkout flow.
layout: schema
name: Affirm Transaction
properties_list:
- description: A unique identifier representing the transaction, assigned by Affirm upon authorization.
  name: id
  type: string
- description: A unique identifier referencing the Checkout object that originated this transaction.
  name: checkout_id
  type: string
- description: Identifies the order within the merchant's order management system, used for reconciliation.
  name: order_id
  type: string
- description: Current lifecycle state of the transaction.
  name: status
  type: string
- description: The original amount financed to the customer, expressed in the smallest currency unit (e.g., cents for USD).
  name: amount
  type: integer
- description: The cumulative amount refunded to the customer from this transaction, in the smallest currency unit.
  name: amount_refunded
  type: integer
- description: The ISO 4217 currency code for this transaction.
  name: currency
  type: string
- description: The timestamp when the transaction was created, in RFC 3339 format.
  name: created
  type: string
- description: The timestamp after which the transaction authorization expires and can no longer be captured, in RFC 3339 format.
  name: authorization_expiration
  type: string
- description: A unique identifier of the financing provider for this transaction.
  name: provider_id
  type: integer
- description: Indicates whether tax was paid by the financing provider. Applicable to Affirm Connect integrations only.
  name: remove_tax
  type: boolean
- description: Array of TransactionEvent objects documenting the full history of actions taken on this transaction.
  name: events
  type: array
- description: A JWT signing the JSON response body. When PII is included in the response, this token is also encrypted.
  name: token
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/affirm-transaction-schema.json
slug: affirm-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://affirm.com/schemas/affirm/transaction.json\",\n  \"title\": \"Affirm Transaction\",\n  \"description\": \"Represents an Affirm payment transaction, capturing the full lifecycle from authorization through capture, refund, and void. Transactions are created by exchanging a checkout token via the Transactions API after a customer completes the Affirm checkout flow.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"status\", \"amount\", \"currency\", \"created\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier representing the transaction, assigned by Affirm upon authorization.\"\n    },\n    \"checkout_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier referencing the Checkout object that originated this transaction.\"\n    },\n    \"order_id\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Identifies the order within the merchant's order management system, used for reconciliation.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle state of the transaction.\",\n      \"enum\": [\"authorized\", \"captured\", \"voided\", \"refunded\", \"partially_refunded\"]\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"The original amount financed to the customer, expressed in the smallest currency unit (e.g., cents for USD).\",\n      \"minimum\": 0\n    },\n    \"amount_refunded\": {\n      \"type\": \"integer\",\n      \"description\": \"The cumulative amount refunded to the customer from this transaction, in the smallest currency unit.\",\n      \"minimum\": 0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 4217 currency code for this transaction.\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"examples\": [\"USD\", \"CAD\", \"GBP\"]\n    },\n    \"created\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the transaction was created, in RFC 3339 format.\"\n    },\n    \"authorization_expiration\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp after which the transaction authorization expires and can no longer be captured, in RFC 3339 format.\"\n    },\n    \"provider_id\": {\n      \"type\": \"integer\",\n      \"description\": \"A unique identifier of the financing provider for this transaction.\"\n    },\n    \"remove_tax\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether tax was paid by the financing provider. Applicable to Affirm Connect integrations only.\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Array of TransactionEvent objects documenting the full history of actions taken on this transaction.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TransactionEvent\"\
  \n      }\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"A JWT signing the JSON response body. When PII is included in the response, this token is also encrypted.\"\n    }\n  },\n  \"$defs\": {\n    \"TransactionEvent\": {\n      \"type\": \"object\",\n      \"description\": \"A single event in the lifecycle of a transaction documenting an action such as authorization, capture, refund, or void.\",\n      \"required\": [\"id\", \"type\", \"amount\", \"currency\", \"created\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"A unique identifier for this transaction event.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of action represented by this event.\",\n          \"enum\": [\"auth\", \"capture\", \"refund\", \"void\", \"update\"]\n        },\n        \"amount\": {\n          \"type\": \"integer\",\n          \"description\": \"The monetary\
  \ amount associated with this event in the smallest currency unit.\",\n          \"minimum\": 0\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"The ISO 4217 currency code for this event.\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"fee\": {\n          \"type\": \"integer\",\n          \"description\": \"The Affirm transaction fee charged for this event, in the smallest currency unit.\",\n          \"minimum\": 0\n        },\n        \"created\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp when this event was created, in RFC 3339 format.\"\n        },\n        \"reference_id\": {\n          \"type\": \"string\",\n          \"description\": \"An external reference identifier for this event, such as a merchant capture or refund reference.\"\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"description\": \"Arbitrary\
  \ key-value metadata associated with this event.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"SettlementEvent\": {\n      \"type\": \"object\",\n      \"description\": \"A disbursement line item from Affirm to the merchant, associated with a specific transaction event.\",\n      \"required\": [\"id\", \"transaction_id\", \"amount\", \"currency\", \"created\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"A unique identifier for this settlement event.\"\n        },\n        \"transaction_id\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the transaction this settlement event is associated with.\"\n        },\n        \"transaction_event_id\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the specific transaction event that triggered this settlement.\"\n        },\n        \"\
  amount\": {\n          \"type\": \"integer\",\n          \"description\": \"The net disbursement amount in the smallest currency unit.\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"The ISO 4217 currency code for this settlement.\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"created\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when this settlement event was created, in RFC 3339 format.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of settlement event, corresponding to the originating transaction action.\",\n          \"enum\": [\"capture\", \"refund\", \"void\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/affirm-transaction-schema.json
tags: []
title: Affirm Transaction
---
