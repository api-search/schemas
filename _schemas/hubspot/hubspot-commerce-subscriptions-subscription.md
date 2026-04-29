---
description: A HubSpot commerce subscription record.
layout: schema
name: Subscription
properties_list:
- description: The unique identifier for the subscription.
  name: id
  type: string
- description: The subscription's properties as key-value pairs.
  name: properties
  type: object
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
- description: ''
  name: archived
  type: boolean
- description: ''
  name: associations
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-commerce-subscriptions-subscription-schema.json
slug: hubspot-commerce-subscriptions-subscription
source_filename: hubspot-commerce-subscriptions-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A HubSpot commerce subscription record.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the subscription.\",\n      \"example\": \"500123\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The subscription's properties as key-value pairs.\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"associations\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"Subscription\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-commerce-subscriptions-subscription-schema.json
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
title: Subscription
---
