---
description: Confirmation of a submitted lead referral
layout: schema
name: LeadReferralResponse
properties_list:
- description: Unique identifier for the submitted lead
  name: lead_id
  type: string
- description: Status of the lead submission
  name: status
  type: string
- description: Timestamp when the lead was submitted
  name: created_at
  type: string
- description: Team or person the lead has been assigned to
  name: assigned_to
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-lead-referral-response-schema.json
slug: api-connect-lead-referral-response
source_filename: api-connect-lead-referral-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-lead-referral-response-schema.json\",\n  \"title\": \"LeadReferralResponse\",\n  \"description\": \"Confirmation of a submitted lead referral\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lead_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the submitted lead\",\n      \"example\": \"lead-500234\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the lead submission\",\n      \"enum\": [\n        \"submitted\",\n        \"assigned\",\n        \"contacted\"\n      ],\n      \"example\": \"submitted\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the lead was submitted\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n  \
  \  },\n    \"assigned_to\": {\n      \"type\": \"string\",\n      \"description\": \"Team or person the lead has been assigned to\",\n      \"example\": \"Allianz Sales Team\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-lead-referral-response-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: LeadReferralResponse
---
