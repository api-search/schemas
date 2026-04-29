---
description: ''
layout: schema
name: ClaimFeature
properties_list:
- description: Name of the insurance claim.
  name: name
  type: string
- description: Status code of the insurance claim.
  name: statusCode
  type: string
- description: Status of the insurance claim.
  name: status
  type: string
- description: Status description of the insurance claim.
  name: statusDescription
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-loyalty-insurance-claim-feature-schema.json
slug: mastercard-loyalty-insurance-claim-feature
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClaimFeature\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the insurance claim.\"\n    },\n    \"statusCode\": {\n      \"type\": \"string\",\n      \"description\": \"Status code of the insurance claim.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the insurance claim.\"\n    },\n    \"statusDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Status description of the insurance claim.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-loyalty-insurance-claim-feature-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ClaimFeature
---
