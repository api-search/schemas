---
description: Contact information for shipping or billing, including name, address, email, and phone number.
layout: schema
name: ContactObject
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: address
  type: object
- description: Email address for the contact.
  name: email
  type: string
- description: Phone number for the contact in E.164 format.
  name: phone_number
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/checkout-contact-object-schema.json
slug: checkout-contact-object
source_filename: checkout-contact-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-contact-object-schema.json\",\n  \"title\": \"ContactObject\",\n  \"description\": \"Contact information for shipping or billing, including name, address, email, and phone number.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"$ref\": \"#/components/schemas/NameObject\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/AddressObject\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address for the contact.\",\n      \"example\": \"merchant@example.com\"\n    },\n    \"phone_number\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number for the contact in E.164 format.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-contact-object-schema.json
tags: []
title: ContactObject
---
