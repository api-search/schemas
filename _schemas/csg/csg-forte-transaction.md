---
description: Schema representing a payment transaction in the CSG Forte payment processing platform.
layout: schema
name: CSG Forte Payment Transaction
properties_list:
- description: Unique transaction identifier in trn_XXXXX format
  name: transaction_id
  type: string
- description: Location identifier where the transaction was processed
  name: location_id
  type: string
- description: Transaction action type
  name: action
  type: string
- description: Transaction amount in USD
  name: authorization_amount
  type: number
- description: Authorization code returned by the card issuer
  name: authorization_code
  type: string
- description: User or system that entered the transaction
  name: entered_by
  type: string
- description: Merchant-assigned order reference number
  name: order_number
  type: string
- description: ISO 8601 timestamp when transaction was received
  name: received_date
  type: string
- description: Date the transaction was processed
  name: transaction_date
  type: string
- description: ''
  name: response
  type: object
- description: ''
  name: billing_address
  type: object
- description: ''
  name: card
  type: object
- description: ''
  name: echeck
  type: object
- description: Token referencing a stored customer record
  name: customer_token
  type: string
- description: Token referencing a stored payment method
  name: paymethod_token
  type: string
- description: ID of the recurring schedule this transaction belongs to
  name: schedule_id
  type: string
- description: Custom extended transaction data fields
  name: xdata
  type: object
provider_name: CSG Systems
provider_slug: csg
schema_file: json-schema/csg-forte-transaction-schema.json
slug: csg-forte-transaction
source_filename: csg-forte-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.forte.net/v3/schemas/transaction\",\n  \"title\": \"CSG Forte Payment Transaction\",\n  \"description\": \"Schema representing a payment transaction in the CSG Forte payment processing platform.\",\n  \"type\": \"object\",\n  \"required\": [\"transaction_id\", \"action\", \"authorization_amount\"],\n  \"properties\": {\n    \"transaction_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction identifier in trn_XXXXX format\",\n      \"pattern\": \"^trn_[A-Za-z0-9]+$\"\n    },\n    \"location_id\": {\n      \"type\": \"string\",\n      \"description\": \"Location identifier where the transaction was processed\",\n      \"pattern\": \"^loc_[A-Za-z0-9]+$\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction action type\",\n      \"enum\": [\"sale\", \"authorize\", \"capture\", \"void\", \"credit\", \"force\", \"verify\"\
  ]\n    },\n    \"authorization_amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Transaction amount in USD\",\n      \"minimum\": 0.01\n    },\n    \"authorization_code\": {\n      \"type\": \"string\",\n      \"description\": \"Authorization code returned by the card issuer\"\n    },\n    \"entered_by\": {\n      \"type\": \"string\",\n      \"description\": \"User or system that entered the transaction\"\n    },\n    \"order_number\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant-assigned order reference number\"\n    },\n    \"received_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when transaction was received\"\n    },\n    \"transaction_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the transaction was processed\"\n    },\n    \"response\": {\n      \"$ref\": \"#/$defs/TransactionResponse\"\n\
  \    },\n    \"billing_address\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"card\": {\n      \"$ref\": \"#/$defs/CardInfo\"\n    },\n    \"echeck\": {\n      \"$ref\": \"#/$defs/EcheckInfo\"\n    },\n    \"customer_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token referencing a stored customer record\"\n    },\n    \"paymethod_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token referencing a stored payment method\"\n    },\n    \"schedule_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the recurring schedule this transaction belongs to\"\n    },\n    \"xdata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom extended transaction data fields\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"TransactionResponse\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"environment\": {\n          \"type\": \"string\",\n     \
  \     \"enum\": [\"live\", \"sandbox\"]\n        },\n        \"response_type\": {\n          \"type\": \"string\",\n          \"description\": \"A=Approved, D=Declined, E=Error, F=Force, U=Undetermined\",\n          \"enum\": [\"A\", \"D\", \"E\", \"F\", \"U\"]\n        },\n        \"response_code\": {\n          \"type\": \"string\",\n          \"description\": \"Processor response code\"\n        },\n        \"response_desc\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable response description\"\n        },\n        \"authorization_code\": {\n          \"type\": \"string\"\n        },\n        \"avs_result\": {\n          \"type\": \"string\",\n          \"description\": \"Address Verification System result code\"\n        },\n        \"cvv_result\": {\n          \"type\": \"string\",\n          \"description\": \"Card Verification Value check result\"\n        }\n      }\n    },\n    \"CardInfo\": {\n      \"type\": \"object\",\n      \"properties\"\
  : {\n        \"card_type\": {\n          \"type\": \"string\",\n          \"enum\": [\"visa\", \"mstr\", \"disc\", \"amex\", \"jcb\", \"dine\", \"enrt\"]\n        },\n        \"name_on_card\": {\n          \"type\": \"string\"\n        },\n        \"masked_account_number\": {\n          \"type\": \"string\",\n          \"description\": \"Masked PAN, e.g., XXXX-XXXX-XXXX-1234\",\n          \"pattern\": \"^X{4}-X{4}-X{4}-[0-9]{4}$\"\n        },\n        \"expire_month\": {\n          \"type\": \"string\",\n          \"pattern\": \"^(0[1-9]|1[0-2])$\"\n        },\n        \"expire_year\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{4}$\"\n        }\n      }\n    },\n    \"EcheckInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"account_type\": {\n          \"type\": \"string\",\n          \"enum\": [\"checking\", \"savings\"]\n        },\n        \"masked_account_number\": {\n          \"type\": \"string\"\n        },\n        \"routing_number\"\
  : {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{9}$\",\n          \"description\": \"9-digit ABA routing number\"\n        },\n        \"sec_code\": {\n          \"type\": \"string\",\n          \"description\": \"NACHA Standard Entry Class code\",\n          \"enum\": [\"PPD\", \"CCD\", \"WEB\", \"TEL\", \"ARC\", \"BOC\", \"POP\", \"RCK\"]\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"first_name\": { \"type\": \"string\" },\n        \"last_name\": { \"type\": \"string\" },\n        \"company_name\": { \"type\": \"string\" },\n        \"physical_address\": { \"type\": \"string\" },\n        \"locality\": { \"type\": \"string\", \"description\": \"City\" },\n        \"region\": { \"type\": \"string\", \"description\": \"State/province\" },\n        \"postal_code\": { \"type\": \"string\" },\n        \"country_code\": { \"type\": \"string\", \"default\": \"US\", \"pattern\": \"^[A-Z]{2}$\" }\n      }\n\
  \    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/csg/refs/heads/main/json-schema/csg-forte-transaction-schema.json
tags:
- Billing
- Customer Engagement
- Payments
- Revenue Management
- Telecom
title: CSG Forte Payment Transaction
---
