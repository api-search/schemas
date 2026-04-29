---
description: Transaction Identifier containing CFC Indicator the key and value pair.
layout: schema
name: TransactionIdentifier
properties_list:
- description: Actual value depending on the 'CFC Indicator' subject to the following validations 1. For ARN, Min Length is 23, Max Length is 23 and Data Type is N. 2. For BRN, Min Length is 6, Max Length is 9 and D
  name: cfcValue
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-confirmed-fraud-transaction-identifier-schema.json
slug: mastercard-confirmed-fraud-transaction-identifier
source_filename: mastercard-confirmed-fraud-transaction-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactionIdentifier\",\n  \"type\": \"object\",\n  \"description\": \"Transaction Identifier containing CFC Indicator the key and value pair.\",\n  \"properties\": {\n    \"cfcValue\": {\n      \"type\": \"string\",\n      \"description\": \"Actual value depending on the 'CFC Indicator' subject to the following validations 1. For ARN, Min Length is 23, Max Length is 23 and Data Type is N. 2. For BRN, Min Length is 6, Max Length is 9 and Data Type is AN. 3. For TRC, Min Length is 6, Max Length is 6 and Data Type is N. 4. For SER, Min Length is 9, Max Length is 9 and Data Type is N.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-confirmed-fraud-transaction-identifier-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: TransactionIdentifier
---
