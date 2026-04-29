---
description: ''
layout: schema
name: PermanentAddress
properties_list:
- description: Date since when the referenced address is defined as the permanent address. <br/> Format - It is expressed in ISO 8601 - `YYYY-MM-DD`
  name: permanentAddressFrom
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-permanent-address-schema.json
slug: mastercard-card-issuance-permanent-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PermanentAddress\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permanentAddressFrom\": {\n      \"type\": \"string\",\n      \"description\": \"Date since when the referenced address is defined as the permanent address.  <br/> Format - It is expressed in ISO 8601 - `YYYY-MM-DD`\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-permanent-address-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: PermanentAddress
---
