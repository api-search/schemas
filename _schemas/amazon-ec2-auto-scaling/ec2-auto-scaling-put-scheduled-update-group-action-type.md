---
description: PutScheduledUpdateGroupActionType schema from Auto Scaling
layout: schema
name: PutScheduledUpdateGroupActionType
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: ScheduledActionName
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
schema_file: json-schema/ec2-auto-scaling-put-scheduled-update-group-action-type-schema.json
slug: ec2-auto-scaling-put-scheduled-update-group-action-type
source_filename: ec2-auto-scaling-put-scheduled-update-group-action-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-put-scheduled-update-group-action-type-schema.json\",\n  \"title\": \"PutScheduledUpdateGroupActionType\",\n  \"description\": \"PutScheduledUpdateGroupActionType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"ScheduledActionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of this scaling action.\"\n        }\n      ]\n    },\n    \"Time\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"This property is no longer used.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"<p>The date and time for this action to start, in YYYY-MM-DDThh:mm:ssZ format in UTC/GMT only and in quotes (for example, <code>\\\"2021-06-01T00:00:00Z\\\"</code>).</p> <p>If you specify <code>Recurrence</code> and <code>StartTime</code>, Amazon EC2 Auto Scaling performs the action at this time, and then performs the action based on the specified recurrence.</p>\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"The date and time for the recurring schedule to end, in UTC. For example, <code>\\\"2021-06-01T00:00:00Z\\\"\
  </code>.\"\n        }\n      ]\n    },\n    \"Recurrence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>The recurring schedule for this action. This format consists of five fields separated by white spaces: [Minute] [Hour] [Day_of_Month] [Month_of_Year] [Day_of_Week]. The value must be in quotes (for example, <code>\\\"30 0 1 1,6,12 *\\\"</code>). For more information about this format, see <a href=\\\"http://crontab.org\\\">Crontab</a>.</p> <p>When <code>StartTime</code> and <code>EndTime</code> are specified with <code>Recurrence</code>, they form the boundaries of when the recurring action starts and stops.</p> <p>Cron expressions use Universal Coordinated Time (UTC) by default.</p>\"\n        }\n      ]\n    },\n    \"MinSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupMinSize\"\n        },\n        {\n          \"description\"\
  : \"The minimum size of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"MaxSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupMaxSize\"\n        },\n        {\n          \"description\": \"The maximum size of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"DesiredCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupDesiredCapacity\"\n        },\n        {\n          \"description\": \"<p>The desired capacity is the initial capacity of the Auto Scaling group after the scheduled action runs and the capacity it attempts to maintain. It can scale beyond this capacity if you add more scaling conditions. </p> <note> <p>You must specify at least one of the following properties: <code>MaxSize</code>, <code>MinSize</code>, or <code>DesiredCapacity</code>. </p> </note>\"\n        }\n      ]\n    },\n    \"TimeZone\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>Specifies the time zone for a cron expression. If a time zone is not provided, UTC is used by default. </p> <p>Valid values are the canonical names of the IANA time zones, derived from the IANA Time Zone Database (such as <code>Etc/GMT+9</code> or <code>Pacific/Tahiti</code>). For more information, see <a href=\\\"https://en.wikipedia.org/wiki/List_of_tz_database_time_zones\\\">https://en.wikipedia.org/wiki/List_of_tz_database_time_zones</a>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\",\n    \"ScheduledActionName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-put-scheduled-update-group-action-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: PutScheduledUpdateGroupActionType
---
