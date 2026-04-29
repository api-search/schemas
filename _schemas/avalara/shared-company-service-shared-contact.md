---
description: SharedContact schema from Avalara API
layout: schema
name: SharedContact
properties_list:
- description: ''
  name: contactId
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: isPrimary
  type: boolean
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/shared-company-service-shared-contact-schema.json
slug: shared-company-service-shared-contact
source_filename: shared-company-service-shared-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/shared-company-service-shared-contact-schema.json\",\n  \"title\": \"SharedContact\",\n  \"description\": \"SharedContact schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contactId\": {\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    },\n    \"phone\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"isPrimary\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/shared-company-service-shared-contact-schema.json
tags:
- Taxes
title: SharedContact
---
