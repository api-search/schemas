---
description: An EDI transaction record for Rite Aid vendor integration using ANSI X12 standards
layout: schema
name: Rite Aid EDI Transaction
properties_list:
- description: ANSI X12 transaction set identifier
  name: transactionSetId
  type: string
- description: Human-readable transaction name
  name: transactionName
  type: string
- description: ANSI X12 version
  name: version
  type: string
- description: Sender identification
  name: sender
  type: object
- description: Receiver identification
  name: receiver
  type: object
- description: Interchange control number
  name: controlNumber
  type: string
- description: Transaction date
  name: date
  type: string
- description: Transaction time (HHMM)
  name: time
  type: string
- description: Transaction processing status
  name: status
  type: string
provider_name: Rite Aid
provider_slug: rite-aid
schema_file: json-schema/rite-aid-edi-transaction-schema.json
slug: rite-aid-edi-transaction
source_filename: rite-aid-edi-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/rite-aid/blob/main/json-schema/rite-aid-edi-transaction-schema.json\",\n  \"title\": \"Rite Aid EDI Transaction\",\n  \"description\": \"An EDI transaction record for Rite Aid vendor integration using ANSI X12 standards\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionSetId\": {\n      \"type\": \"string\",\n      \"description\": \"ANSI X12 transaction set identifier\",\n      \"enum\": [\"810\", \"820\", \"832\", \"846\", \"850\", \"855\", \"856\", \"860\", \"865\", \"997\"]\n    },\n    \"transactionName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable transaction name\",\n      \"examples\": [\n        \"Invoice\",\n        \"Payment Order\",\n        \"Price/Sales Catalog\",\n        \"Inventory Inquiry/Advice\",\n        \"Purchase Order\",\n        \"Purchase Order Acknowledgment\",\n        \"Ship Notice/Manifest\"\
  ,\n        \"Purchase Order Change Request\",\n        \"Purchase Order Change Acknowledgment\",\n        \"Functional Acknowledgment\"\n      ]\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"ANSI X12 version\",\n      \"enum\": [\"4010\", \"5010\"]\n    },\n    \"sender\": {\n      \"type\": \"object\",\n      \"description\": \"Sender identification\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"EDI sender ID\"\n        },\n        \"qualifier\": {\n          \"type\": \"string\",\n          \"description\": \"ID qualifier\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\"id\", \"qualifier\"]\n    },\n    \"receiver\": {\n      \"type\": \"object\",\n      \"description\": \"Receiver identification\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"EDI receiver ID (Rite\
  \ Aid's ID)\"\n        },\n        \"qualifier\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\"id\", \"qualifier\"]\n    },\n    \"controlNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Interchange control number\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Transaction date\"\n    },\n    \"time\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction time (HHMM)\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction processing status\",\n      \"enum\": [\"Pending\", \"Sent\", \"Acknowledged\", \"Accepted\", \"Rejected\", \"Error\"]\n    }\n  },\n  \"required\": [\"transactionSetId\", \"version\", \"sender\", \"receiver\", \"controlNumber\", \"date\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rite-aid/refs/heads/main/json-schema/rite-aid-edi-transaction-schema.json
tags:
- EDI
- Fortune 500
- Health
- Pharmacy
- Prescriptions
- Retail
title: Rite Aid EDI Transaction
---
