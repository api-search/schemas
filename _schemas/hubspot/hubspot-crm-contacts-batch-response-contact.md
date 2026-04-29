---
description: Results from a batch operation on contacts.
layout: schema
name: BatchResponseContact
properties_list:
- description: The status of the batch operation.
  name: status
  type: string
- description: ''
  name: results
  type: array
- description: ''
  name: completedAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-contacts-batch-response-contact-schema.json
slug: hubspot-crm-contacts-batch-response-contact
source_filename: hubspot-crm-contacts-batch-response-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Results from a batch operation on contacts.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the batch operation.\",\n      \"example\": \"active\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"properties\": {\n            \"key\": \"value\"\n          },\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\",\n          \"archived\": true,\n          \"associations\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A HubSpot contact record.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the contact.\",\n            \"example\": \"500123\"\
  \n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"The contact's properties as key-value pairs.\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time the contact was created.\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time the contact was last updated.\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the contact has been archived.\",\n            \"example\": true\n          },\n          \"associations\": {\n            \"type\": \"object\",\n   \
  \         \"description\": \"The contact's associations with other CRM objects.\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        }\n      }\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchResponseContact\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-contacts-batch-response-contact-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: BatchResponseContact
---
