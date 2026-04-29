---
description: Information about the next page of results
layout: schema
name: NextPage
properties_list:
- description: The cursor token for the next page
  name: after
  type: string
- description: A direct link to the next page
  name: link
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-domains-next-page-schema.json
slug: hubspot-domains-next-page
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Information about the next page of results\",\n  \"properties\": {\n    \"after\": {\n      \"type\": \"string\",\n      \"description\": \"The cursor token for the next page\",\n      \"example\": \"NTI1Cg%3D%3D\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"description\": \"A direct link to the next page\",\n      \"example\": \"?after=NTI1Cg%3D%3D\"\n    }\n  },\n  \"required\": [\n    \"after\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NextPage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-domains-next-page-schema.json
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
