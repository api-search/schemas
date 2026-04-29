---
description: StartCrawlerScheduleRequest schema from Amazon Glue API
layout: schema
name: StartCrawlerScheduleRequest
properties_list:
- description: ''
  name: CrawlerName
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-start-crawler-schedule-request-schema.json
slug: glue-start-crawler-schedule-request
source_filename: glue-start-crawler-schedule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-crawler-schedule-request-schema.json\",\n  \"title\": \"StartCrawlerScheduleRequest\",\n  \"description\": \"StartCrawlerScheduleRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrawlerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Name of the crawler to schedule.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CrawlerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-crawler-schedule-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StartCrawlerScheduleRequest
---
