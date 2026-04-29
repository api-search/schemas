---
description: ''
layout: schema
name: NewApplication
properties_list:
- description: Echo back the input application form number.
  name: formNumber
  type: string
- description: System generated unique application number while on-boarding the client.
  name: number
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-new-application-schema.json
slug: mastercard-card-issuance-new-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NewApplication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"formNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Echo back the input application form number.\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"System generated unique application number while on-boarding the client.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-new-application-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: NewApplication
---
