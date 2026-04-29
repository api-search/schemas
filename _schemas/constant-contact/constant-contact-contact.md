---
description: Schema for a Constant Contact V3 contact resource.
layout: schema
name: Constant Contact Contact
properties_list:
- description: Unique identifier for the contact.
  name: contact_id
  type: string
- description: ''
  name: email_address
  type: object
- description: ''
  name: first_name
  type: string
- description: ''
  name: last_name
  type: string
- description: ''
  name: job_title
  type: string
- description: ''
  name: company_name
  type: string
- description: ''
  name: phone_numbers
  type: array
- description: ''
  name: sms_channel
  type: object
- description: ''
  name: street_addresses
  type: array
- description: ''
  name: custom_fields
  type: array
- description: ''
  name: list_memberships
  type: array
- description: ''
  name: taggings
  type: array
- description: ''
  name: create_source
  type: string
- description: ''
  name: update_source
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: deleted_at
  type: string
provider_name: Constant Contact
provider_slug: constant-contact
schema_file: json-schema/constant-contact-contact-schema.json
slug: constant-contact-contact
source_filename: constant-contact-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/json-schema/constant-contact-contact-schema.json\",\n  \"title\": \"Constant Contact Contact\",\n  \"description\": \"Schema for a Constant Contact V3 contact resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contact_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the contact.\"\n    },\n    \"email_address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"address\": { \"type\": \"string\", \"format\": \"email\" },\n        \"permission_to_send\": {\n          \"type\": \"string\",\n          \"enum\": [\"explicit\", \"implicit\", \"pending_confirmation\", \"temp_hold\", \"unsubscribed\"]\n        },\n        \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"updated_at\": { \"type\": \"string\"\
  , \"format\": \"date-time\" },\n        \"opt_in_source\": { \"type\": \"string\" },\n        \"opt_in_date\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"opt_out_source\": { \"type\": \"string\" },\n        \"opt_out_date\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"opt_out_reason\": { \"type\": \"string\" },\n        \"confirm_status\": { \"type\": \"string\" }\n      },\n      \"required\": [\"address\"]\n    },\n    \"first_name\": { \"type\": \"string\", \"maxLength\": 50 },\n    \"last_name\": { \"type\": \"string\", \"maxLength\": 50 },\n    \"job_title\": { \"type\": \"string\", \"maxLength\": 50 },\n    \"company_name\": { \"type\": \"string\", \"maxLength\": 50 },\n    \"phone_numbers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"phone_number_id\": { \"type\": \"string\" },\n          \"phone_number\": { \"type\": \"string\" },\n          \"kind\": { \"type\"\
  : \"string\", \"enum\": [\"home_phone\", \"work_phone\", \"mobile_phone\", \"other_phone\"] }\n        }\n      }\n    },\n    \"sms_channel\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"full_sms_address\": { \"type\": \"string\" },\n        \"sms_channel_consents\": { \"type\": \"array\" }\n      }\n    },\n    \"street_addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"street_address_id\": { \"type\": \"string\" },\n          \"kind\": { \"type\": \"string\", \"enum\": [\"home\", \"work\", \"other\"] },\n          \"street\": { \"type\": \"string\" },\n          \"city\": { \"type\": \"string\" },\n          \"state\": { \"type\": \"string\" },\n          \"postal_code\": { \"type\": \"string\" },\n          \"country\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"custom_fields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n\
  \        \"properties\": {\n          \"custom_field_id\": { \"type\": \"string\" },\n          \"value\": { \"type\": \"string\" }\n        },\n        \"required\": [\"custom_field_id\", \"value\"]\n      }\n    },\n    \"list_memberships\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\", \"format\": \"uuid\" }\n    },\n    \"taggings\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\", \"format\": \"uuid\" }\n    },\n    \"create_source\": { \"type\": \"string\", \"enum\": [\"Contact\", \"Account\"] },\n    \"update_source\": { \"type\": \"string\", \"enum\": [\"Contact\", \"Account\"] },\n    \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"updated_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"deleted_at\": { \"type\": \"string\", \"format\": \"date-time\" }\n  },\n  \"required\": [\"email_address\", \"create_source\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/constant-contact/refs/heads/main/json-schema/constant-contact-contact-schema.json
tags:
- Campaigns
- Contacts
- Email Marketing
- Events
- Reporting
- SMS
- Surveys
title: Constant Contact Contact
---
