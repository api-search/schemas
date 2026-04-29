---
description: The details of a schedule.
layout: schema
name: ScheduleSummary
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: GroupName
  type: object
- description: ''
  name: LastModificationDate
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: Target
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-schedule-summary-schema.json
slug: amazon-eventbridge-scheduler-schedule-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-schedule-summary-schema.json\",\n  \"title\": \"ScheduleSummary\",\n  \"description\": \"The details of a schedule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the schedule.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreationDate\"\n        },\n        {\n          \"description\": \"The time at which the schedule was created.\"\n        }\n      ]\n    },\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleGroupName\"\n        },\n\
  \        {\n          \"description\": \"The name of the schedule group associated with this schedule.\"\n        }\n      ]\n    },\n    \"LastModificationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModificationDate\"\n        },\n        {\n          \"description\": \"The time at which the schedule was last modified.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the schedule.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleState\"\n        },\n        {\n          \"description\": \"Specifies whether the schedule is enabled or disabled.\"\n        }\n      ]\n    },\n    \"Target\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetSummary\"\n        },\n        {\n          \"description\"\
  : \"The schedule's target details.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-schedule-summary-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: ScheduleSummary
---
