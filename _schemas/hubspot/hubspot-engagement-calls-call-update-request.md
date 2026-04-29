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
schema_file: json-schema/hubspot-engagement-calls-call-update-request-schema.json
slug: hubspot-engagement-calls-call-update-request
source_filename: hubspot-engagement-calls-call-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a call\",\n  \"properties\": {\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The call properties to update\",\n      \"example\": {\n        \"hs_call_title\": \"Updated Discovery Call\",\n        \"hs_call_disposition\": \"connected\"\n      }\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallUpdateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-calls-call-update-request-schema.json
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
