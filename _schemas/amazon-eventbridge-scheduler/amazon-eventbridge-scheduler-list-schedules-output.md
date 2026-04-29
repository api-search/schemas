---
description: ListSchedulesOutput schema from Amazon EventBridge Scheduler
layout: schema
name: ListSchedulesOutput
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Schedules
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-list-schedules-output-schema.json
slug: amazon-eventbridge-scheduler-list-schedules-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-list-schedules-output-schema.json\",\n  \"title\": \"ListSchedulesOutput\",\n  \"description\": \"ListSchedulesOutput schema from Amazon EventBridge Scheduler\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Indicates whether there are additional results to retrieve. If the value is null, there are no more results.\"\n        }\n      ]\n    },\n    \"Schedules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleList\"\n        },\n        {\n          \"description\": \"The schedules that match the specified criteria.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"Schedules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-list-schedules-output-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: ListSchedulesOutput
---
