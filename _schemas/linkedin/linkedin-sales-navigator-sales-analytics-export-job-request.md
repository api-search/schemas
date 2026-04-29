---
description: SalesAnalyticsExportJobRequest from LinkedIn API
layout: schema
name: SalesAnalyticsExportJobRequest
properties_list:
- description: Sales Navigator contract URN
  name: contract
  type: string
- description: Start date of the exported data (milliseconds since epoch)
  name: startAt
  type: integer
- description: End date of the exported data (milliseconds since epoch)
  name: endAt
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-sales-navigator-sales-analytics-export-job-request-schema.json
slug: linkedin-sales-navigator-sales-analytics-export-job-request
source_filename: linkedin-sales-navigator-sales-analytics-export-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-sales-analytics-export-job-request-schema.json\",\n  \"title\": \"SalesAnalyticsExportJobRequest\",\n  \"description\": \"SalesAnalyticsExportJobRequest from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contract\": {\n      \"type\": \"string\",\n      \"description\": \"Sales Navigator contract URN\",\n      \"example\": \"urn:li:salesContract:12345\"\n    },\n    \"startAt\": {\n      \"type\": \"integer\",\n      \"description\": \"Start date of the exported data (milliseconds since epoch)\",\n      \"example\": 1638316800000\n    },\n    \"endAt\": {\n      \"type\": \"integer\",\n      \"description\": \"End date of the exported data (milliseconds since epoch)\",\n      \"example\": 1640908800000\n    }\n  },\n  \"required\": [\n    \"contract\",\n    \"startAt\"\
  ,\n    \"endAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-sales-analytics-export-job-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: SalesAnalyticsExportJobRequest
---
