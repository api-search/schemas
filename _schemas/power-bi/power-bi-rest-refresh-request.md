---
description: Request body for an enhanced dataset refresh
layout: schema
name: RefreshRequest
properties_list:
- description: The type of processing to perform
  name: type
  type: string
- description: Determines whether objects are committed in batches or only when complete
  name: commitMode
  type: string
- description: Maximum number of threads to run in parallel
  name: maxParallelism
  type: integer
- description: Number of times to retry on failure
  name: retryCount
  type: integer
- description: Specific tables or partitions to refresh
  name: objects
  type: array
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-refresh-request-schema.json
slug: power-bi-rest-refresh-request
source_filename: power-bi-rest-refresh-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RefreshRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for an enhanced dataset refresh\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of processing to perform\"\n    },\n    \"commitMode\": {\n      \"type\": \"string\",\n      \"description\": \"Determines whether objects are committed in batches or only when complete\"\n    },\n    \"maxParallelism\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of threads to run in parallel\"\n    },\n    \"retryCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times to retry on failure\"\n    },\n    \"objects\": {\n      \"type\": \"array\",\n      \"description\": \"Specific tables or partitions to refresh\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-refresh-request-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: RefreshRequest
---
