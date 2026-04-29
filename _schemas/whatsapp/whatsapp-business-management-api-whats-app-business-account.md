---
description: WhatsAppBusinessAccount from WhatsApp API
layout: schema
name: WhatsAppBusinessAccount
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: currency
  type: string
- description: ''
  name: timezone_id
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: business_verification_status
  type: string
- description: ''
  name: message_template_namespace
  type: string
- description: ''
  name: owner_business
  type: object
- description: ''
  name: primary_funding_id
  type: string
- description: ''
  name: purchase_order_number
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-business-management-api-whats-app-business-account-schema.json
slug: whatsapp-business-management-api-whats-app-business-account
source_filename: whatsapp-business-management-api-whats-app-business-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-whats-app-business-account-schema.json\",\n  \"title\": \"WhatsAppBusinessAccount\",\n  \"description\": \"WhatsAppBusinessAccount from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Business\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"timezone_id\": {\n      \"type\": \"string\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\"\n    \
  \  ],\n      \"example\": \"ACTIVE\"\n    },\n    \"business_verification_status\": {\n      \"type\": \"string\",\n      \"example\": \"sent\"\n    },\n    \"message_template_namespace\": {\n      \"type\": \"string\",\n      \"example\": \"Example Business\"\n    },\n    \"owner_business\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"primary_funding_id\": {\n      \"type\": \"string\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"purchase_order_number\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-whats-app-business-account-schema.json
tags: []
title: WhatsAppBusinessAccount
---
