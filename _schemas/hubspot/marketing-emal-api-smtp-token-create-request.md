---
description: Request body for creating an SMTP token
layout: schema
name: SmtpTokenCreateRequest
properties_list:
- description: The name for the email campaign
  name: campaignName
  type: string
- description: Whether to create contacts for recipients who don't exist
  name: createContact
  type: boolean
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/marketing-emal-api-smtp-token-create-request-schema.json
slug: marketing-emal-api-smtp-token-create-request
source_filename: marketing-emal-api-smtp-token-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/marketing-emal-api-smtp-token-create-request-schema.json\",\n  \"title\": \"SmtpTokenCreateRequest\",\n  \"description\": \"Request body for creating an SMTP token\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaignName\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the email campaign\",\n      \"example\": \"Order Confirmation Emails\"\n    },\n    \"createContact\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to create contacts for recipients who don't exist\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"campaignName\",\n    \"createContact\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/marketing-emal-api-smtp-token-create-request-schema.json
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
title: SmtpTokenCreateRequest
---
