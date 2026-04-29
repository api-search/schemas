---
description: Pagination information for forward navigation
layout: schema
name: ForwardPaging
properties_list:
- description: Information about the next page of results
  name: next
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-domains-forward-paging-schema.json
slug: hubspot-domains-forward-paging
source_filename: hubspot-domains-forward-paging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Pagination information for forward navigation\",\n  \"properties\": {\n    \"next\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the next page of results\",\n      \"properties\": {\n        \"after\": {\n          \"type\": \"string\",\n          \"description\": \"The cursor token for the next page\",\n          \"example\": \"NTI1Cg%3D%3D\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"description\": \"A direct link to the next page\",\n          \"example\": \"?after=NTI1Cg%3D%3D\"\n        }\n      },\n      \"required\": [\n        \"after\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ForwardPaging\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-domains-forward-paging-schema.json
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
title: ForwardPaging
---
