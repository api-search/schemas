---
description: ''
layout: schema
name: UserName
properties_list:
- description: Denotes the first name of the user.
  name: firstName
  type: string
- description: Denotes the last name of the user.
  name: lastName
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-carbon-calculator-experience-user-name-schema.json
slug: mastercard-carbon-calculator-experience-user-name
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserName\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"Denotes the first name of the user.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Denotes the last name of the user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-carbon-calculator-experience-user-name-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: UserName
---
