---
description: Contact schema from Adyen API
layout: schema
name: Contact
properties_list:
- description: The individual's email address.
  name: email
  type: string
- description: The individual's first name.
  name: firstName
  type: string
- description: The infix in the individual's name, if any.
  name: infix
  type: string
- description: The individual's last name.
  name: lastName
  type: string
- description: The individual's phone number, specified as 10-14 digits with an optional `+` prefix.
  name: phoneNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-contact-schema.json
slug: management-contact
source_filename: management-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-contact-schema.json\",\n  \"title\": \"Contact\",\n  \"description\": \"Contact schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"description\": \"The individual's email address.\",\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"description\": \"The individual's first name.\",\n      \"type\": \"string\"\n    },\n    \"infix\": {\n      \"description\": \"The infix in the individual's name, if any.\",\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"description\": \"The individual's last name.\",\n      \"type\": \"string\"\n    },\n    \"phoneNumber\": {\n      \"description\": \"The individual's phone number, specified as 10-14 digits with an optional `+` prefix.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-contact-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Contact
---
