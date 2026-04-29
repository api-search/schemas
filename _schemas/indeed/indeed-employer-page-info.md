---
description: Pagination information for list responses.
layout: schema
name: PageInfo
properties_list:
- description: Whether there are more results available.
  name: hasNextPage
  type: boolean
- description: Whether there are previous results available.
  name: hasPreviousPage
  type: boolean
- description: Cursor for the first item in the current page.
  name: startCursor
  type: string
- description: Cursor for the last item in the current page.
  name: endCursor
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-page-info-schema.json
slug: indeed-employer-page-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageInfo\",\n  \"type\": \"object\",\n  \"description\": \"Pagination information for list responses.\",\n  \"properties\": {\n    \"hasNextPage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether there are more results available.\"\n    },\n    \"hasPreviousPage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether there are previous results available.\"\n    },\n    \"startCursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the first item in the current page.\"\n    },\n    \"endCursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the last item in the current page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-page-info-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: PageInfo
---
