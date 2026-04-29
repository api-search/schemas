---
description: ''
layout: schema
name: BaseAccount
properties_list:
- description: Indicates given account is default account or not
  name: default
  type: boolean
- description: Currency of the account. <br> Values - 3 letter alphabetic currency codes in `ISO 4217` <br/>
  name: currency
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-base-account-schema.json
slug: mastercard-card-issuance-base-account
source_filename: mastercard-card-issuance-base-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BaseAccount\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"default\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates given account is default account or not\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency of the account. <br> Values - 3 letter alphabetic currency codes in `ISO 4217` <br/>\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-base-account-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: BaseAccount
---
