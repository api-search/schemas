---
description: UpdateScheduleInput schema from Amazon EventBridge Scheduler
layout: schema
name: UpdateScheduleInput
properties_list:
- description: ''
  name: ActionAfterCompletion
  type: object
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: EndDate
  type: object
- description: ''
  name: FlexibleTimeWindow
  type: object
- description: ''
  name: GroupName
  type: object
- description: ''
  name: KmsKeyArn
  type: object
- description: ''
  name: ScheduleExpression
  type: object
- description: ''
  name: ScheduleExpressionTimezone
  type: object
- description: ''
  name: StartDate
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: Target
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-update-schedule-input-schema.json
slug: amazon-eventbridge-scheduler-update-schedule-input
source_filename: amazon-eventbridge-scheduler-update-schedule-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-update-schedule-input-schema.json\",\n  \"title\": \"UpdateScheduleInput\",\n  \"description\": \"UpdateScheduleInput schema from Amazon EventBridge Scheduler\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActionAfterCompletion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionAfterCompletion\"\n        },\n        {\n          \"description\": \"Specifies the action that EventBridge Scheduler applies to the schedule after the schedule completes invoking the target.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \" Unique, case-sensitive identifier you provide to ensure the\
  \ idempotency of the request. If you do not specify a client token, EventBridge Scheduler uses a randomly generated token for the request to ensure idempotency. \"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description you specify for the schedule.\"\n        }\n      ]\n    },\n    \"EndDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndDate\"\n        },\n        {\n          \"description\": \"The date, in UTC, before which the schedule can invoke its target. Depending on the schedule's recurrence expression, invocations might stop on, or before, the <code>EndDate</code> you specify. EventBridge Scheduler ignores <code>EndDate</code> for one-time schedules.\"\n        }\n      ]\n    },\n    \"FlexibleTimeWindow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlexibleTimeWindow\"\
  \n        },\n        {\n          \"description\": \"Allows you to configure a time window during which EventBridge Scheduler invokes the schedule.\"\n        }\n      ]\n    },\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleGroupName\"\n        },\n        {\n          \"description\": \"The name of the schedule group with which the schedule is associated. You must provide this value in order for EventBridge Scheduler to find the schedule you want to update. If you omit this value, EventBridge Scheduler assumes the group is associated to the default group.\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyArn\"\n        },\n        {\n          \"description\": \"The ARN for the customer managed KMS key that that you want EventBridge Scheduler to use to encrypt and decrypt your data.\"\n        }\n      ]\n    },\n    \"ScheduleExpression\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleExpression\"\n        },\n        {\n          \"description\": \"<p> The expression that defines when the schedule runs. The following formats are supported. </p> <ul> <li> <p> <code>at</code> expression - <code>at(yyyy-mm-ddThh:mm:ss)</code> </p> </li> <li> <p> <code>rate</code> expression - <code>rate(value unit)</code> </p> </li> <li> <p> <code>cron</code> expression - <code>cron(fields)</code> </p> </li> </ul> <p> You can use <code>at</code> expressions to create one-time schedules that invoke a target once, at the time and in the time zone, that you specify. You can use <code>rate</code> and <code>cron</code> expressions to create recurring schedules. Rate-based schedules are useful when you want to invoke a target at regular intervals, such as every 15 minutes or every five days. Cron-based schedules are useful when you want to invoke a target periodically at a specific time, such as at 8:00 am (UTC+0)\
  \ every 1st day of the month. </p> <p> A <code>cron</code> expression consists of six fields separated by white spaces: <code>(minutes hours day_of_month month day_of_week year)</code>. </p> <p> A <code>rate</code> expression consists of a <i>value</i> as a positive integer, and a <i>unit</i> with the following options: <code>minute</code> | <code>minutes</code> | <code>hour</code> | <code>hours</code> | <code>day</code> | <code>days</code> </p> <p> For more information and examples, see <a href=\\\"https://docs.aws.amazon.com/scheduler/latest/UserGuide/schedule-types.html\\\">Schedule types on EventBridge Scheduler</a> in the <i>EventBridge Scheduler User Guide</i>. </p>\"\n        }\n      ]\n    },\n    \"ScheduleExpressionTimezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleExpressionTimezone\"\n        },\n        {\n          \"description\": \"The timezone in which the scheduling expression is evaluated.\"\n        }\n      ]\n    },\n\
  \    \"StartDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartDate\"\n        },\n        {\n          \"description\": \"The date, in UTC, after which the schedule can begin invoking its target. Depending on the schedule's recurrence expression, invocations might occur on, or after, the <code>StartDate</code> you specify. EventBridge Scheduler ignores <code>StartDate</code> for one-time schedules.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleState\"\n        },\n        {\n          \"description\": \"Specifies whether the schedule is enabled or disabled.\"\n        }\n      ]\n    },\n    \"Target\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Target\"\n        },\n        {\n          \"description\": \"The schedule target. You can use this operation to change the target that your schedule invokes.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"FlexibleTimeWindow\",\n    \"ScheduleExpression\",\n    \"Target\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-update-schedule-input-schema.json
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
title: UpdateScheduleInput
---
