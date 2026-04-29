---
description: A Commerce charge representing a cryptocurrency payment request. Charges generate blockchain addresses where customers can send payments, and track the payment lifecycle from creation through confirmation or failure.
layout: schema
name: Coinbase Commerce Charge
properties_list:
- description: Unique charge identifier assigned by Coinbase Commerce
  name: id
  type: string
- description: Short unique code for the charge, used in hosted URLs
  name: code
  type: string
- description: Name describing what the charge is for
  name: name
  type: string
- description: Detailed description of the charge
  name: description
  type: string
- description: Pricing model for the charge
  name: pricing_type
  type: string
- description: Price in a local fiat currency (required for fixed_price)
  name: local_price
  type: object
- description: Pricing expressed in multiple currencies
  name: pricing
  type: object
- description: Blockchain addresses generated for receiving payment, keyed by network name
  name: addresses
  type: object
- description: URL for the hosted payment page
  name: hosted_url
  type: string
- description: URL to redirect to after successful payment
  name: redirect_url
  type: string
- description: URL to redirect to if payment is cancelled
  name: cancel_url
  type: string
- description: Payments received for this charge
  name: payments
  type: array
- description: Chronological list of status changes
  name: timeline
  type: array
- description: Custom key-value metadata for integrations
  name: metadata
  type: object
- description: When the charge was created
  name: created_at
  type: string
- description: When the charge was confirmed
  name: confirmed_at
  type: string
- description: When the charge expires
  name: expires_at
  type: string
provider_name: Coinbase
provider_slug: coinbase
schema_file: json-schema/coinbase-charge-schema.json
slug: coinbase-charge
source_filename: coinbase-charge-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://coinbase.com/schemas/coinbase/charge.json\",\n  \"title\": \"Coinbase Commerce Charge\",\n  \"description\": \"A Commerce charge representing a cryptocurrency payment request. Charges generate blockchain addresses where customers can send payments, and track the payment lifecycle from creation through confirmation or failure.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"description\", \"pricing_type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique charge identifier assigned by Coinbase Commerce\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Short unique code for the charge, used in hosted URLs\",\n      \"pattern\": \"^[A-Z0-9]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name describing what the charge is for\",\n      \"minLength\": 1,\n      \"\
  maxLength\": 200\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the charge\",\n      \"maxLength\": 1000\n    },\n    \"pricing_type\": {\n      \"type\": \"string\",\n      \"description\": \"Pricing model for the charge\",\n      \"enum\": [\"no_price\", \"fixed_price\"]\n    },\n    \"local_price\": {\n      \"$ref\": \"#/$defs/Money\",\n      \"description\": \"Price in a local fiat currency (required for fixed_price)\"\n    },\n    \"pricing\": {\n      \"type\": \"object\",\n      \"description\": \"Pricing expressed in multiple currencies\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Money\"\n      }\n    },\n    \"addresses\": {\n      \"type\": \"object\",\n      \"description\": \"Blockchain addresses generated for receiving payment, keyed by network name\",\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"description\": \"Blockchain address\"\n      }\n    },\n  \
  \  \"hosted_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the hosted payment page\"\n    },\n    \"redirect_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to redirect to after successful payment\"\n    },\n    \"cancel_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to redirect to if payment is cancelled\"\n    },\n    \"payments\": {\n      \"type\": \"array\",\n      \"description\": \"Payments received for this charge\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Payment\"\n      }\n    },\n    \"timeline\": {\n      \"type\": \"array\",\n      \"description\": \"Chronological list of status changes\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TimelineEntry\"\n      }\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom key-value metadata for integrations\",\n      \"additionalProperties\"\
  : {\n        \"type\": \"string\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the charge was created\"\n    },\n    \"confirmed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the charge was confirmed\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the charge expires\"\n    }\n  },\n  \"$defs\": {\n    \"Money\": {\n      \"type\": \"object\",\n      \"description\": \"A monetary value with currency\",\n      \"required\": [\"amount\", \"currency\"],\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"string\",\n          \"description\": \"Monetary amount as a decimal string\",\n          \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"Currency code (e.g.,\
  \ USD, BTC, ETH)\",\n          \"minLength\": 1,\n          \"maxLength\": 10\n        }\n      }\n    },\n    \"Payment\": {\n      \"type\": \"object\",\n      \"description\": \"A blockchain payment received for a charge\",\n      \"properties\": {\n        \"network\": {\n          \"type\": \"string\",\n          \"description\": \"Blockchain network the payment was made on\"\n        },\n        \"transaction_id\": {\n          \"type\": \"string\",\n          \"description\": \"Blockchain transaction hash\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Payment confirmation status\",\n          \"enum\": [\"PENDING\", \"CONFIRMED\", \"FAILED\"]\n        },\n        \"value\": {\n          \"$ref\": \"#/$defs/Money\",\n          \"description\": \"Payment value\"\n        },\n        \"block\": {\n          \"type\": \"object\",\n          \"description\": \"Blockchain block information\",\n          \"properties\": {\n         \
  \   \"height\": {\n              \"type\": \"integer\",\n              \"description\": \"Block height\",\n              \"minimum\": 0\n            },\n            \"hash\": {\n              \"type\": \"string\",\n              \"description\": \"Block hash\"\n            },\n            \"confirmations_required\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of confirmations required\",\n              \"minimum\": 1\n            },\n            \"confirmations\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of confirmations received\",\n              \"minimum\": 0\n            }\n          }\n        }\n      }\n    },\n    \"TimelineEntry\": {\n      \"type\": \"object\",\n      \"description\": \"A status change entry in the charge timeline\",\n      \"properties\": {\n        \"time\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the status change\
  \ occurred\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Status at this point in the timeline\",\n          \"enum\": [\"NEW\", \"PENDING\", \"COMPLETED\", \"EXPIRED\", \"UNRESOLVED\", \"RESOLVED\", \"CANCELED\"]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/json-schema/coinbase-charge-schema.json
tags:
- Blockchain
- Cryptocurrency
- Custody
- Exchange
- Onramp
- Payments
- Trading
- Wallet
- Web3
title: Coinbase Commerce Charge
---
