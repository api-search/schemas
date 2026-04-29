---
description: VerificationRequest schema from AgeChecker.Net API
layout: schema
name: VerificationRequest
properties_list:
- description: Customer first name.
  name: first_name
  type: string
- description: Customer last name.
  name: last_name
  type: string
- description: Customer date of birth (YYYY-MM-DD).
  name: birth_date
  type: string
- description: Street address.
  name: address
  type: string
- description: City.
  name: city
  type: string
- description: State or province code.
  name: state
  type: string
- description: Postal/ZIP code.
  name: zip
  type: string
- description: ISO 3166-1 alpha-2 country code.
  name: country
  type: string
- description: Customer email address.
  name: email
  type: string
- description: Customer phone number.
  name: phone
  type: string
- description: Customer's IP address.
  name: ip_address
  type: string
- description: Minimum age required (default is 21 for alcohol, 18 for tobacco).
  name: minimum_age
  type: integer
provider_name: AgeChecker.Net
provider_slug: agechecker-net
schema_file: json-schema/age-verification-verification-request-schema.json
slug: age-verification-verification-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/json-schema/age-verification-verification-request-schema.json\",\n  \"title\": \"VerificationRequest\",\n  \"description\": \"VerificationRequest schema from AgeChecker.Net API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Customer first name.\",\n      \"example\": \"Example Name\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Customer last name.\",\n      \"example\": \"Example Name\"\n    },\n    \"birth_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Customer date of birth (YYYY-MM-DD).\",\n      \"example\": \"2025-03-15\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Street address.\",\n      \"example\": \"example_value\"\
  \n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City.\",\n      \"example\": \"example_value\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province code.\",\n      \"example\": \"example_value\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"Postal/ZIP code.\",\n      \"example\": \"example_value\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code.\",\n      \"default\": \"US\",\n      \"example\": \"example_value\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Customer email address.\",\n      \"example\": \"admin@example.com\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Customer phone number.\",\n      \"example\": \"example_value\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Customer's IP address.\",\n      \"example\": \"example_value\"\n    },\n    \"minimum_age\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum age required (default is 21 for alcohol, 18 for tobacco).\",\n      \"default\": 21,\n      \"example\": 1\n    }\n  },\n  \"required\": [\n    \"first_name\",\n    \"last_name\",\n    \"birth_date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/json-schema/age-verification-verification-request-schema.json
tags:
- Age Verification
- Identity
- Compliance
- Regulatory
- E-Commerce
title: VerificationRequest
---
