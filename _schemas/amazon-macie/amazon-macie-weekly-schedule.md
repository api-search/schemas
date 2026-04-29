---
description: Specifies a weekly recurrence pattern for running a classification job.
layout: schema
name: WeeklySchedule
properties_list:
- description: ''
  name: dayOfWeek
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-weekly-schedule-schema.json
slug: amazon-macie-weekly-schedule
source_filename: amazon-macie-weekly-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-weekly-schedule-schema.json\",\n  \"title\": \"WeeklySchedule\",\n  \"description\": \"Specifies a weekly recurrence pattern for running a classification job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dayOfWeek\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DayOfWeek\"\n        },\n        {\n          \"description\": \"The day of the week when Amazon Macie runs the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-weekly-schedule-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: WeeklySchedule
---
