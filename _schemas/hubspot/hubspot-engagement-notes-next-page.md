---
description: Information about the next page
layout: schema
name: NextPage
properties_list:
- description: Cursor for the next page
  name: after
  type: string
- description: Link to the next page
  name: link
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-notes-next-page-schema.json
slug: hubspot-engagement-notes-next-page
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Information about the next page\",\n  \"properties\": {\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page\",\n      \"example\": \"MTAyNA%3D%3D\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"description\": \"Link to the next page\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    }\n  },\n  \"required\": [\n    \"after\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NextPage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-notes-next-page-schema.json
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
title: NextPage
---
