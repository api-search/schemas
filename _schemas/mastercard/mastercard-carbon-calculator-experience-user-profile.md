---
description: The request object for enrolling a new user to Carbon Calculator Experience API.
layout: schema
name: UserProfile
properties_list:
- description: Name of the card-holder. (format- First Name Last Name)
  name: cardholderName
  type: string
- description: User locale which is registered with Issuer.
  name: locale
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-carbon-calculator-experience-user-profile-schema.json
slug: mastercard-carbon-calculator-experience-user-profile
source_filename: mastercard-carbon-calculator-experience-user-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserProfile\",\n  \"type\": \"object\",\n  \"description\": \"The request object for enrolling a new user to Carbon Calculator Experience API.\",\n  \"properties\": {\n    \"cardholderName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the card-holder. (format- First Name Last Name)\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"User locale which is registered with Issuer.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-carbon-calculator-experience-user-profile-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: UserProfile
---
