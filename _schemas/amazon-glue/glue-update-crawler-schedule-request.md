---
description: UpdateCrawlerScheduleRequest schema from Amazon Glue API
layout: schema
name: UpdateCrawlerScheduleRequest
properties_list:
- description: ''
  name: CrawlerName
  type: object
- description: ''
  name: Schedule
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-crawler-schedule-request-schema.json
slug: glue-update-crawler-schedule-request
source_filename: glue-update-crawler-schedule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-crawler-schedule-request-schema.json\",\n  \"title\": \"UpdateCrawlerScheduleRequest\",\n  \"description\": \"UpdateCrawlerScheduleRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrawlerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the crawler whose schedule to update.\"\n        }\n      ]\n    },\n    \"Schedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CronExpression\"\n        },\n        {\n          \"description\": \"The updated <code>cron</code> expression used to specify the schedule (see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/monitor-data-warehouse-schedule.html\\\">Time-Based\
  \ Schedules for Jobs and Crawlers</a>. For example, to run something every day at 12:15 UTC, you would specify: <code>cron(15 12 * * ? *)</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CrawlerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-crawler-schedule-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateCrawlerScheduleRequest
---
