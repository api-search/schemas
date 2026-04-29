---
description: Specifies a monthly recurrence pattern for running a classification job.
layout: schema
name: MonthlySchedule
properties_list:
- description: ''
  name: dayOfMonth
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-monthly-schedule-schema.json
slug: amazon-macie-monthly-schedule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-monthly-schedule-schema.json\",\n  \"title\": \"MonthlySchedule\",\n  \"description\": \"Specifies a monthly recurrence pattern for running a classification job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dayOfMonth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"<p>The numeric day of the month when Amazon Macie runs the job. This value can be an integer from 1 through 31.</p> <p>If this value exceeds the number of days in a certain month, Macie doesn't run the job that month. Macie runs the job only during months that have the specified day. For example, if this value is 31 and a month has only 30 days, Macie doesn't run the job that month. To run the job every month, specify a value\
  \ that's less than 29.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-monthly-schedule-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: MonthlySchedule
---
