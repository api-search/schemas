---
description: SalesAnalyticsExportJob from LinkedIn API
layout: schema
name: SalesAnalyticsExportJob
properties_list:
- description: A unique identifier for the job
  name: id
  type: integer
- description: Current status of the export job
  name: status
  type: string
- description: URL for downloading the exported data when job is completed
  name: downloadUrl
  type: string
- description: Expiration timestamp of the download URL
  name: expireAt
  type: integer
- description: Number of rows in the exported data
  name: rowCount
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-sales-navigator-sales-analytics-export-job-schema.json
slug: linkedin-sales-navigator-sales-analytics-export-job
source_filename: linkedin-sales-navigator-sales-analytics-export-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-sales-analytics-export-job-schema.json\",\n  \"title\": \"SalesAnalyticsExportJob\",\n  \"description\": \"SalesAnalyticsExportJob from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"A unique identifier for the job\",\n      \"example\": 987654321\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENQUEUED\",\n        \"PROCESSING\",\n        \"COMPLETED\",\n        \"FAILED_DUE_TO_EXCEEDED_FILE_SIZE_ERROR\",\n        \"FAILED_DUE_TO_TIMED_OUT\",\n        \"FAILED_DUE_TO_DATA_DELAY\",\n        \"FAILED_DUE_TO_INTERNAL_ERROR\"\n      ],\n      \"description\": \"Current status of the export job\",\n      \"example\": \"COMPLETED\"\n    },\n    \"downloadUrl\": {\n  \
  \    \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"URL for downloading the exported data when job is completed\",\n      \"example\": \"https://media.licdn.com/exports/analytics_123.csv\"\n    },\n    \"expireAt\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Expiration timestamp of the download URL\",\n      \"example\": 1640200000\n    },\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Number of rows in the exported data\",\n      \"example\": 5000\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-sales-analytics-export-job-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: SalesAnalyticsExportJob
---
