---
description: Request body for GDPR deletion
layout: schema
name: GdprDeleteRequest
properties_list:
- description: The ID of the call to permanently delete
  name: objectId
  type: string
- description: The property used as the identifier
  name: idProperty
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-calls-api-gdpr-delete-request-schema.json
slug: engagement-calls-api-gdpr-delete-request
source_filename: engagement-calls-api-gdpr-delete-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-gdpr-delete-request-schema.json\",\n  \"title\": \"GdprDeleteRequest\",\n  \"description\": \"Request body for GDPR deletion\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the call to permanently delete\",\n      \"example\": \"512\"\n    },\n    \"idProperty\": {\n      \"type\": \"string\",\n      \"description\": \"The property used as the identifier\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"objectId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-gdpr-delete-request-schema.json
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
title: GdprDeleteRequest
---
