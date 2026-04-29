---
description: A group of dimension filters applied to the query.
layout: schema
name: DimensionFilterGroup
properties_list:
- description: How filters within this group are combined.
  name: groupType
  type: string
- description: Filters within this group.
  name: filters
  type: array
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-dimension-filter-group-schema.json
slug: google-search-console-dimension-filter-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DimensionFilterGroup\",\n  \"type\": \"object\",\n  \"description\": \"A group of dimension filters applied to the query.\",\n  \"properties\": {\n    \"groupType\": {\n      \"type\": \"string\",\n      \"description\": \"How filters within this group are combined.\"\n    },\n    \"filters\": {\n      \"type\": \"array\",\n      \"description\": \"Filters within this group.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-dimension-filter-group-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: DimensionFilterGroup
---
