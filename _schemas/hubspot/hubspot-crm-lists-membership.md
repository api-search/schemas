---
description: A list membership record.
layout: schema
name: Membership
properties_list:
- description: The ID of the CRM record that is a member of the list.
  name: recordId
  type: string
- description: The date and time the record was added to the list.
  name: addedAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-lists-membership-schema.json
slug: hubspot-crm-lists-membership
source_filename: hubspot-crm-lists-membership-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A list membership record.\",\n  \"properties\": {\n    \"recordId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the CRM record that is a member of the list.\",\n      \"example\": \"500123\"\n    },\n    \"addedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the record was added to the list.\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Membership\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-lists-membership-schema.json
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
title: Membership
---
