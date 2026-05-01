---
description: StopCrawlerScheduleRequest schema from Amazon Glue API
layout: schema
name: StopCrawlerScheduleRequest
properties_list:
- description: ''
  name: CrawlerName
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-stop-crawler-schedule-request-schema.json
slug: glue-stop-crawler-schedule-request
source_filename: glue-stop-crawler-schedule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-stop-crawler-schedule-request-schema.json\",\n  \"title\": \"StopCrawlerScheduleRequest\",\n  \"description\": \"StopCrawlerScheduleRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrawlerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Name of the crawler whose schedule state to set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CrawlerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-stop-crawler-schedule-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StopCrawlerScheduleRequest
---
