---
description: Licensing statistics summary for the authenticated member
layout: schema
name: LicenseStatsResponse
properties_list:
- description: Total number of licensing events in the requested period
  name: nb_results
  type: integer
- description: Aggregated licensing statistics by content type
  name: stock_user
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-license-stats-response-schema.json
slug: adobe-creative-suite-stock-license-stats-response
source_filename: adobe-creative-suite-stock-license-stats-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-license-stats-response-schema.json\",\n  \"title\": \"LicenseStatsResponse\",\n  \"description\": \"Licensing statistics summary for the authenticated member\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nb_results\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of licensing events in the requested period\",\n      \"example\": 1920\n    },\n    \"stock_user\": {\n      \"type\": \"object\",\n      \"description\": \"Aggregated licensing statistics by content type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-license-stats-response-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: LicenseStatsResponse
---
