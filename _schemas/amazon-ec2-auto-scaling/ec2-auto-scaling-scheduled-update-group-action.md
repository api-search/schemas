---
description: Describes a scheduled scaling action.
layout: schema
name: ScheduledUpdateGroupAction
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: ScheduledActionName
  type: object
- description: ''
  name: ScheduledActionARN
  type: object
- description: ''
  name: Time
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: Recurrence
  type: object
- description: ''
  name: MinSize
  type: object
- description: ''
  name: MaxSize
  type: object
- description: ''
  name: DesiredCapacity
  type: object
- description: ''
  name: TimeZone
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-scheduled-update-group-action-schema.json
slug: ec2-auto-scaling-scheduled-update-group-action
source_filename: ec2-auto-scaling-scheduled-update-group-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scheduled-update-group-action-schema.json\",\n  \"title\": \"ScheduledUpdateGroupAction\",\n  \"description\": \"Describes a scheduled scaling action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"ScheduledActionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the scheduled action.\"\n        }\n      ]\n    },\n    \"ScheduledActionARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the scheduled action.\"\n        }\n      ]\n    },\n    \"Time\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"This property is no longer used.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"The date and time in UTC for this action to start. For example, <code>\\\"2019-06-01T00:00:00Z\\\"</code>. \"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"The date and time in UTC for the recurring schedule to end. For example, <code>\\\"2019-06-01T00:00:00Z\\\"</code>. \"\n        }\n      ]\n    },\n    \"Recurrence\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>The recurring schedule for the action, in Unix cron syntax format.</p> <p>When <code>StartTime</code> and <code>EndTime</code> are specified with <code>Recurrence</code>, they form the boundaries of when the recurring action starts and stops.</p>\"\n        }\n      ]\n    },\n    \"MinSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupMinSize\"\n        },\n        {\n          \"description\": \"The minimum size of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"MaxSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupMaxSize\"\n        },\n        {\n          \"description\": \"The maximum size of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"DesiredCapacity\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/AutoScalingGroupDesiredCapacity\"\n        },\n        {\n          \"description\": \"The desired capacity is the initial capacity of the Auto Scaling group after the scheduled action runs and the capacity it attempts to maintain.\"\n        }\n      ]\n    },\n    \"TimeZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The time zone for the cron expression.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scheduled-update-group-action-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: ScheduledUpdateGroupAction
---
