---
description: Indicates who has submitted the transaction. If only Issuer submitted the transaction then value of this field will be 'ISSUER'. If only Acquirer submitted the transaction then value of this field will be 'ACQUIRER'. If both the parties have submitted the transaction then the value of this field will be 'BOTH'.
layout: schema
name: Initiator
properties_list: []
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-suspected-fraud-initiator-schema.json
slug: mastercard-suspected-fraud-initiator
source_filename: mastercard-suspected-fraud-initiator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Initiator\",\n  \"type\": \"string\",\n  \"description\": \"Indicates who has submitted the transaction. If only Issuer submitted the transaction then value of this field will be 'ISSUER'. If only Acquirer submitted the transaction then value of this field will be 'ACQUIRER'. If both the parties have submitted the transaction then the value of this field will be 'BOTH'.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-suspected-fraud-initiator-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Initiator
---
