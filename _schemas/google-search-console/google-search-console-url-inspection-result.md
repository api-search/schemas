---
description: The aggregated inspection result for a URL, including index status, crawl information, mobile usability, and rich results.
layout: schema
name: UrlInspectionResult
properties_list:
- description: Link to the URL inspection result in the Search Console UI.
  name: inspectionResultLink
  type: string
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-url-inspection-result-schema.json
slug: google-search-console-url-inspection-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UrlInspectionResult\",\n  \"type\": \"object\",\n  \"description\": \"The aggregated inspection result for a URL, including index status, crawl information, mobile usability, and rich results.\",\n  \"properties\": {\n    \"inspectionResultLink\": {\n      \"type\": \"string\",\n      \"description\": \"Link to the URL inspection result in the Search Console UI.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-url-inspection-result-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: UrlInspectionResult
---
