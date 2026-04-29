---
description: Specifies the recurrence pattern for running a classification job.
layout: schema
name: JobScheduleFrequency
properties_list:
- description: ''
  name: dailySchedule
  type: object
- description: ''
  name: monthlySchedule
  type: object
- description: ''
  name: weeklySchedule
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-job-schedule-frequency-schema.json
slug: amazon-macie-job-schedule-frequency
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-schedule-frequency-schema.json\",\n  \"title\": \"JobScheduleFrequency\",\n  \"description\": \"Specifies the recurrence pattern for running a classification job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dailySchedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DailySchedule\"\n        },\n        {\n          \"description\": \"Specifies a daily recurrence pattern for running the job.\"\n        }\n      ]\n    },\n    \"monthlySchedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MonthlySchedule\"\n        },\n        {\n          \"description\": \"Specifies a monthly recurrence pattern for running the job.\"\n        }\n      ]\n    },\n    \"weeklySchedule\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/WeeklySchedule\"\n        },\n        {\n          \"description\": \"Specifies a weekly recurrence pattern for running the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-job-schedule-frequency-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: JobScheduleFrequency
---
