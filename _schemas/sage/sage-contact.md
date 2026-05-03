---
description: A customer or supplier contact in Sage Accounting.
layout: schema
name: Sage Contact
properties_list:
- description: Unique contact identifier
  name: id
  type: string
- description: Display name for the contact
  name: displayed_as
  type: string
- description: Contact full name or company name
  name: name
  type: string
- description: Internal reference code
  name: reference
  type: string
- description: Contact types (CUSTOMER, SUPPLIER, or both)
  name: contact_types
  type: array
- description: Primary email address
  name: email
  type: string
- description: Primary telephone number
  name: telephone
  type: string
- description: Mobile phone number
  name: mobile
  type: string
- description: Website URL
  name: website
  type: string
- description: Postal address
  name: address
  type: object
- description: Current account balance
  name: balance
  type: number
- description: Outstanding unpaid balance
  name: outstanding_balance
  type: number
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Sage
provider_slug: sage
schema_file: json-schema/sage-contact-schema.json
slug: sage-contact
source_filename: sage-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sage/main/json-schema/sage-contact-schema.json\",\n  \"title\": \"Sage Contact\",\n  \"description\": \"A customer or supplier contact in Sage Accounting.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique contact identifier\"\n    },\n    \"displayed_as\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the contact\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact full name or company name\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Internal reference code\"\n    },\n    \"contact_types\": {\n      \"type\": \"array\",\n      \"description\": \"Contact types (CUSTOMER, SUPPLIER, or both)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"id\": {\n            \"type\": \"string\",\n            \"enum\": [\"CUSTOMER\", \"SUPPLIER\"]\n          },\n          \"displayed_as\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary email address\"\n    },\n    \"telephone\": {\n      \"type\": \"string\",\n      \"description\": \"Primary telephone number\"\n    },\n    \"mobile\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile phone number\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Website URL\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"description\": \"Postal address\",\n      \"properties\": {\n        \"address_line_1\": {\"type\": \"string\"},\n        \"address_line_2\": {\"type\": \"string\"},\n        \"city\": {\"type\": \"string\"},\n        \"region\": {\"\
  type\": \"string\"},\n        \"postal_code\": {\"type\": \"string\"},\n        \"country\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\"type\": \"string\"},\n            \"displayed_as\": {\"type\": \"string\"}\n          }\n        }\n      }\n    },\n    \"balance\": {\n      \"type\": \"number\",\n      \"description\": \"Current account balance\"\n    },\n    \"outstanding_balance\": {\n      \"type\": \"number\",\n      \"description\": \"Outstanding unpaid balance\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"contact_types\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sage/refs/heads/main/json-schema/sage-contact-schema.json
tags:
- Accounting
- Business Management
- Cloud Software
- ERP
- Payroll
- HR
title: Sage Contact
---
