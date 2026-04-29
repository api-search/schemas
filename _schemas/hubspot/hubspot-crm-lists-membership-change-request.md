---
description: Request body for adding or removing list members.
layout: schema
name: MembershipChangeRequest
properties_list:
- description: The IDs of records to add to the list.
  name: recordIdsToAdd
  type: array
- description: The IDs of records to remove from the list.
  name: recordIdsToRemove
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-lists-membership-change-request-schema.json
slug: hubspot-crm-lists-membership-change-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for adding or removing list members.\",\n  \"properties\": {\n    \"recordIdsToAdd\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of records to add to the list.\",\n      \"example\": [\n        \"500123\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"recordIdsToRemove\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of records to remove from the list.\",\n      \"example\": [\n        \"500123\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MembershipChangeRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-lists-membership-change-request-schema.json
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
title: MembershipChangeRequest
---
