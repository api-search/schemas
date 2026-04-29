---
description: The details of a schedule group.
layout: schema
name: ScheduleGroupSummary
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationDate
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
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-schedule-group-summary-schema.json
slug: amazon-eventbridge-scheduler-schedule-group-summary
source_filename: amazon-eventbridge-scheduler-schedule-group-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-schedule-group-summary-schema.json\",\n  \"title\": \"ScheduleGroupSummary\",\n  \"description\": \"The details of a schedule group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleGroupArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the schedule group.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreationDate\"\n        },\n        {\n          \"description\": \"The time at which the schedule group was created.\"\n        }\n      ]\n    },\n    \"LastModificationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModificationDate\"\
  \n        },\n        {\n          \"description\": \"The time at which the schedule group was last modified.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleGroupName\"\n        },\n        {\n          \"description\": \"The name of the schedule group.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleGroupState\"\n        },\n        {\n          \"description\": \"Specifies the state of the schedule group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-schedule-group-summary-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: ScheduleGroupSummary
---
