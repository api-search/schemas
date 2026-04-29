---
description: Response for listing Search Console sites.
layout: schema
name: SitesListResponse
properties_list:
- description: List of verified sites.
  name: siteEntry
  type: array
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-sites-list-response-schema.json
slug: google-search-console-sites-list-response
source_filename: google-search-console-sites-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SitesListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response for listing Search Console sites.\",\n  \"properties\": {\n    \"siteEntry\": {\n      \"type\": \"array\",\n      \"description\": \"List of verified sites.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-sites-list-response-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: SitesListResponse
---
