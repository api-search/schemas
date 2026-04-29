---
description: Rich results inspection results for a URL.
layout: schema
name: RichResultsInspectionResult
properties_list:
- description: The overall rich results verdict.
  name: verdict
  type: string
- description: A list of detected rich result item types and their status.
  name: detectedItems
  type: array
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-rich-results-inspection-result-schema.json
slug: google-search-console-rich-results-inspection-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RichResultsInspectionResult\",\n  \"type\": \"object\",\n  \"description\": \"Rich results inspection results for a URL.\",\n  \"properties\": {\n    \"verdict\": {\n      \"type\": \"string\",\n      \"description\": \"The overall rich results verdict.\"\n    },\n    \"detectedItems\": {\n      \"type\": \"array\",\n      \"description\": \"A list of detected rich result item types and their status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-rich-results-inspection-result-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: RichResultsInspectionResult
---
