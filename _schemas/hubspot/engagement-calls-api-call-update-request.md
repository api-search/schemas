---
description: Request body for updating a call
layout: schema
name: CallUpdateRequest
properties_list:
- description: The call properties to update
  name: properties
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-calls-api-call-update-request-schema.json
slug: engagement-calls-api-call-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-call-update-request-schema.json\",\n  \"title\": \"CallUpdateRequest\",\n  \"description\": \"Request body for updating a call\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The call properties to update\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"hs_call_title\": \"Updated Discovery Call\",\n        \"hs_call_disposition\": \"connected\"\n      }\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-calls-api-call-update-request-schema.json
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
title: CallUpdateRequest
---
