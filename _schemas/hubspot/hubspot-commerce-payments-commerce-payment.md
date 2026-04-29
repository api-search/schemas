---
description: A commerce payment object representing a payment transaction
layout: schema
name: CommercePayment
properties_list:
- description: The unique identifier of the commerce payment
  name: id
  type: string
- description: The properties of the commerce payment
  name: properties
  type: object
- description: When the commerce payment was created
  name: createdAt
  type: string
- description: When the commerce payment was last updated
  name: updatedAt
  type: string
- description: Whether the commerce payment is archived
  name: archived
  type: boolean
- description: When the commerce payment was archived
  name: archivedAt
  type: string
- description: Associated objects
  name: associations
  type: object
- description: Properties with their value history
  name: propertiesWithHistory
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-payments-commerce-payment-schema.json
slug: hubspot-commerce-payments-commerce-payment
source_filename: hubspot-commerce-payments-commerce-payment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A commerce payment object representing a payment transaction\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the commerce payment\",\n      \"example\": \"500123\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The properties of the commerce payment\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the commerce payment was created\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the commerce payment was last updated\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the commerce\
  \ payment is archived\",\n      \"example\": true\n    },\n    \"archivedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the commerce payment was archived\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"associations\": {\n      \"type\": \"object\",\n      \"description\": \"Associated objects\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"propertiesWithHistory\": {\n      \"type\": \"object\",\n      \"description\": \"Properties with their value history\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"properties\",\n    \"createdAt\",\n    \"updatedAt\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommercePayment\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-payments-commerce-payment-schema.json
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
title: CommercePayment
---
