---
description: CreateScheduleRequest schema from Amazon Glue DataBrew API
layout: schema
name: CreateScheduleRequest
properties_list:
- description: ''
  name: JobNames
  type: object
- description: ''
  name: CronExpression
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-create-schedule-request-schema.json
slug: glue-databrew-create-schedule-request
source_filename: glue-databrew-create-schedule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-create-schedule-request-schema.json\",\n  \"title\": \"CreateScheduleRequest\",\n  \"description\": \"CreateScheduleRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobNameList\"\n        },\n        {\n          \"description\": \"The name or names of one or more jobs to be run.\"\n        }\n      ]\n    },\n    \"CronExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CronExpression\"\n        },\n        {\n          \"description\": \"The date or dates and time or times when the jobs are to be run. For more information, see <a href=\\\"https://docs.aws.amazon.com/databrew/latest/dg/jobs.cron.html\\\">Cron\
  \ expressions</a> in the <i>Glue DataBrew Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags to apply to this schedule.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleName\"\n        },\n        {\n          \"description\": \"A unique name for the schedule. Valid characters are alphanumeric (A-Z, a-z, 0-9), hyphen (-), period (.), and space.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CronExpression\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-create-schedule-request-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: CreateScheduleRequest
---
