---
description: Contact information for a tenant
layout: schema
name: Contact
properties_list:
- description: ''
  name: firstname
  type: string
- description: ''
  name: lastname
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: address1
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: country
  type: string
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/account-management-contact-schema.json
slug: account-management-contact
source_filename: account-management-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-contact-schema.json\",\n  \"title\": \"Contact\",\n  \"description\": \"Contact information for a tenant\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstname\": {\n      \"type\": \"string\",\n      \"example\": \"John\"\n    },\n    \"lastname\": {\n      \"type\": \"string\",\n      \"example\": \"Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"example\": \"john.smith@example.com\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"+1-555-0100\"\n    },\n    \"address1\": {\n      \"type\": \"string\",\n      \"example\": \"123 Main Street\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"example\": \"Springfield\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"US\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-contact-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: Contact
---
