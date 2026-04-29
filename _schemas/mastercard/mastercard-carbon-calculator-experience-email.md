---
description: ''
layout: schema
name: Email
properties_list:
- description: Denotes the type of email (For example, home)
  name: type
  type: string
- description: Denotes email address.
  name: value
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-carbon-calculator-experience-email-schema.json
slug: mastercard-carbon-calculator-experience-email
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Email\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Denotes the  type of email (For example, home)\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Denotes email address.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-carbon-calculator-experience-email-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Email
---
