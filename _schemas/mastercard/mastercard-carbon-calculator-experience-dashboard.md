---
description: ''
layout: schema
name: Dashboard
properties_list:
- description: This is the URL that needs to be rendered in web view with language code send by the issuer appended at the end of the URL.
  name: url
  type: string
- description: Denotes expiry limit for the URL.
  name: expiryInMillis
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-carbon-calculator-experience-dashboard-schema.json
slug: mastercard-carbon-calculator-experience-dashboard
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Dashboard\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"This is the URL that needs to be rendered in web view with language code send by the issuer appended at the end of the URL.\"\n    },\n    \"expiryInMillis\": {\n      \"type\": \"string\",\n      \"description\": \"Denotes expiry limit for the URL.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-carbon-calculator-experience-dashboard-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Dashboard
---
