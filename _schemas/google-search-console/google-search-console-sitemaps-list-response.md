---
description: Response for listing sitemaps.
layout: schema
name: SitemapsListResponse
properties_list:
- description: List of sitemaps for the site.
  name: sitemap
  type: array
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-sitemaps-list-response-schema.json
slug: google-search-console-sitemaps-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SitemapsListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response for listing sitemaps.\",\n  \"properties\": {\n    \"sitemap\": {\n      \"type\": \"array\",\n      \"description\": \"List of sitemaps for the site.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-sitemaps-list-response-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: SitemapsListResponse
---
