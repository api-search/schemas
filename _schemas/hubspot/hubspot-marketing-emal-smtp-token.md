---
description: Represents an SMTP API token for transactional email sending
layout: schema
name: SmtpToken
properties_list:
- description: The unique identifier for the SMTP token
  name: id
  type: string
- description: The name of the email campaign associated with this token
  name: campaignName
  type: string
- description: The ID of the associated email campaign
  name: emailCampaignId
  type: string
- description: Whether sending an email creates a contact if one doesn't exist
  name: createContact
  type: boolean
- description: When the token was created
  name: createdAt
  type: string
- description: The user or application that created the token
  name: createdBy
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-marketing-emal-smtp-token-schema.json
slug: hubspot-marketing-emal-smtp-token
source_filename: hubspot-marketing-emal-smtp-token-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents an SMTP API token for transactional email sending\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the SMTP token\",\n      \"example\": \"smtp-token-abc123\"\n    },\n    \"campaignName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the email campaign associated with this token\",\n      \"example\": \"Password Reset Emails\"\n    },\n    \"emailCampaignId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the associated email campaign\",\n      \"example\": \"campaign-xyz789\"\n    },\n    \"createContact\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether sending an email creates a contact if one doesn't exist\",\n      \"example\": true\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the token was created\",\n      \"format\": \"date-time\"\
  ,\n      \"example\": \"2024-01-15T10:30:00.000Z\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user or application that created the token\",\n      \"example\": \"user@example.com\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"createdAt\",\n    \"createdBy\",\n    \"campaignName\",\n    \"createContact\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SmtpToken\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-marketing-emal-smtp-token-schema.json
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
title: SmtpToken
---
