---
description: Mobile usability inspection results for a URL.
layout: schema
name: MobileUsabilityInspectionResult
properties_list:
- description: The overall mobile usability verdict.
  name: verdict
  type: string
- description: A list of mobile usability issues found.
  name: issues
  type: array
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-mobile-usability-inspection-result-schema.json
slug: google-search-console-mobile-usability-inspection-result
source_filename: google-search-console-mobile-usability-inspection-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MobileUsabilityInspectionResult\",\n  \"type\": \"object\",\n  \"description\": \"Mobile usability inspection results for a URL.\",\n  \"properties\": {\n    \"verdict\": {\n      \"type\": \"string\",\n      \"description\": \"The overall mobile usability verdict.\"\n    },\n    \"issues\": {\n      \"type\": \"array\",\n      \"description\": \"A list of mobile usability issues found.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-mobile-usability-inspection-result-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: MobileUsabilityInspectionResult
---
