---
description: PagingLink from LinkedIn API
layout: schema
name: PagingLink
properties_list:
- description: ''
  name: rel
  type: string
- description: ''
  name: href
  type: string
- description: ''
  name: type
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-insights-paging-link-schema.json
slug: linkedin-marketing-audience-insights-paging-link
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-paging-link-schema.json\",\n  \"title\": \"PagingLink\",\n  \"description\": \"PagingLink from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rel\": {\n      \"type\": \"string\",\n      \"example\": \"next\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"example\": \"/rest/adTargetingEntities?q=typeahead&query=united%20states&start=10&count=10\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"application/json\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-paging-link-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: PagingLink
---
