---
description: ''
layout: schema
name: RegisteredContacts
properties_list:
- description: Fax Number. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: fax
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-registered-contacts-schema.json
slug: mastercard-card-issuance-registered-contacts
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RegisteredContacts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fax\": {\n      \"type\": \"string\",\n      \"description\": \"Fax Number. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-registered-contacts-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: RegisteredContacts
---
