---
description: CrmDataValidationExportJob from LinkedIn API
layout: schema
name: CrmDataValidationExportJob
properties_list:
- description: Export job ID
  name: jobId
  type: integer
- description: Start time of the export
  name: exportStartAt
  type: integer
- description: End time of the export
  name: exportEndAt
  type: integer
- description: Current status of the export job
  name: status
  type: string
- description: URLs for downloading the exported data
  name: downloadUrls
  type: array
- description: Suggested start time for next export
  name: nextExportStartAt
  type: integer
- description: Expiration timestamp for download URLs
  name: expireAt
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-sales-navigator-crm-data-validation-export-job-schema.json
slug: linkedin-sales-navigator-crm-data-validation-export-job
source_filename: linkedin-sales-navigator-crm-data-validation-export-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-crm-data-validation-export-job-schema.json\",\n  \"title\": \"CrmDataValidationExportJob\",\n  \"description\": \"CrmDataValidationExportJob from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Export job ID\",\n      \"example\": 123456789\n    },\n    \"exportStartAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Start time of the export\",\n      \"example\": 1640000000000\n    },\n    \"exportEndAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"nullable\": true,\n      \"description\": \"End time of the export\",\n      \"example\": 1640001000000\n    },\n    \"status\": {\n      \"type\": \"string\"\
  ,\n      \"enum\": [\n        \"PROCESSING\",\n        \"COMPLETED\",\n        \"FAILED_DUE_TO_INTERNAL_ERROR\"\n      ],\n      \"description\": \"Current status of the export job\",\n      \"example\": \"COMPLETED\"\n    },\n    \"downloadUrls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"nullable\": true,\n      \"description\": \"URLs for downloading the exported data\",\n      \"example\": [\n        \"https://media.licdn.com/crm-validation/export_1.csv\",\n        \"https://media.licdn.com/crm-validation/export_2.csv\"\n      ]\n    },\n    \"nextExportStartAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"nullable\": true,\n      \"description\": \"Suggested start time for next export\",\n      \"example\": 1640001000000\n    },\n    \"expireAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"nullable\": true,\n      \"description\": \"Expiration timestamp for download URLs\"\
  ,\n      \"example\": 1640100000000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-crm-data-validation-export-job-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: CrmDataValidationExportJob
---
