---
description: Content type information within a sitemap.
layout: schema
name: WmxSitemapContent
properties_list:
- description: The type of content in this sitemap segment.
  name: type
  type: string
- description: The number of URLs of this type submitted in the sitemap.
  name: submitted
  type: integer
- description: The number of URLs of this type that have been indexed by Google.
  name: indexed
  type: integer
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-wmx-sitemap-content-schema.json
slug: google-search-console-wmx-sitemap-content
source_filename: google-search-console-wmx-sitemap-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WmxSitemapContent\",\n  \"type\": \"object\",\n  \"description\": \"Content type information within a sitemap.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of content in this sitemap segment.\"\n    },\n    \"submitted\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of URLs of this type submitted in the sitemap.\"\n    },\n    \"indexed\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of URLs of this type that have been indexed by Google.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-wmx-sitemap-content-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: WmxSitemapContent
---
