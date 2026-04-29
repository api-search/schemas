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
schema_file: json-schema/marketing-emal-api-next-page-schema.json
slug: marketing-emal-api-next-page
source_filename: marketing-emal-api-next-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/marketing-emal-api-next-page-schema.json\",\n  \"title\": \"NextPage\",\n  \"description\": \"Information about the next page\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page\",\n      \"example\": \"c210cC10b2tlbi1hYmMxMjM%3D\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"description\": \"Link to the next page\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    }\n  },\n  \"required\": [\n    \"after\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/marketing-emal-api-next-page-schema.json
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
