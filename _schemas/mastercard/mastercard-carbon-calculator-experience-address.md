---
description: ''
layout: schema
name: Address
properties_list:
- description: Denotes three-character country code.
  name: countryCode
  type: string
- description: Neighborhood.
  name: locality
  type: string
- description: <p> The postal code in the address is the ZIP code or equivalent and can be an alphanumeric value including whitespace (for example, PE7 8FT). <br><b> Note - Special characters and only whitespace cha
  name: postalCode
  type: string
- description: The state or region or province to which the address belongs.
  name: state
  type: string
- description: City.
  name: city
  type: string
- description: Street Address line1.
  name: line1
  type: string
- description: Street Address line2.
  name: line2
  type: string
- description: Street Address line3.
  name: line3
  type: string
- description: Denotes the type of address. (For example, home or work)
  name: type
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-carbon-calculator-experience-address-schema.json
slug: mastercard-carbon-calculator-experience-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Address\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Denotes three-character country code.\"\n    },\n    \"locality\": {\n      \"type\": \"string\",\n      \"description\": \"Neighborhood.\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"<p> The postal code in the address is the ZIP code or equivalent and can be an alphanumeric value including whitespace (for example, PE7 8FT). <br><b> Note - Special characters and only whitespace characters are not allowed. </b></p>\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state or region or province to which the address belongs.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City.\"\n    },\n    \"line1\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Street Address line1.\"\n    },\n    \"line2\": {\n      \"type\": \"string\",\n      \"description\": \"Street Address line2.\"\n    },\n    \"line3\": {\n      \"type\": \"string\",\n      \"description\": \"Street Address line3.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Denotes the type of address. (For example, home or work)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-carbon-calculator-experience-address-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Address
---
