---
description: UpdateScheduleRequest schema from Amazon Glue DataBrew API
layout: schema
name: UpdateScheduleRequest
properties_list:
- description: ''
  name: JobNames
  type: object
- description: ''
  name: CronExpression
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-update-schedule-request-schema.json
slug: glue-databrew-update-schedule-request
source_filename: glue-databrew-update-schedule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-schedule-request-schema.json\",\n  \"title\": \"UpdateScheduleRequest\",\n  \"description\": \"UpdateScheduleRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobNameList\"\n        },\n        {\n          \"description\": \"The name or names of one or more jobs to be run for this schedule.\"\n        }\n      ]\n    },\n    \"CronExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CronExpression\"\n        },\n        {\n          \"description\": \"The date or dates and time or times when the jobs are to be run. For more information, see <a href=\\\"https://docs.aws.amazon.com/databrew/latest/dg/jobs.cron.html\\\
  \">Cron expressions</a> in the <i>Glue DataBrew Developer Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CronExpression\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-schedule-request-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: UpdateScheduleRequest
---
