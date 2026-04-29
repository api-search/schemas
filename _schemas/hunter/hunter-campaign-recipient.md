---
description: ''
layout: schema
name: CampaignRecipient
properties_list:
- description: Recipient email address.
  name: email
  type: string
- description: Associated lead identifier.
  name: lead_id
  type: '[''integer'', ''null'']'
- description: Current sending status for this recipient.
  name: sending_status
  type: string
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-campaign-recipient-schema.json
slug: hunter-campaign-recipient
source_filename: hunter-campaign-recipient-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CampaignRecipient\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Recipient email address.\"\n    },\n    \"lead_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Associated lead identifier.\"\n    },\n    \"sending_status\": {\n      \"type\": \"string\",\n      \"description\": \"Current sending status for this recipient.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-campaign-recipient-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: CampaignRecipient
---
