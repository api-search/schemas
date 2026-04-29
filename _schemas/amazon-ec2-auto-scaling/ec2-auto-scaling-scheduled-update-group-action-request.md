---
description: Describes information used for one or more scheduled scaling action updates in a <a>BatchPutScheduledUpdateGroupAction</a> operation.
layout: schema
name: ScheduledUpdateGroupActionRequest
properties_list:
- description: ''
  name: ScheduledActionName
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
schema_file: json-schema/ec2-auto-scaling-scheduled-update-group-action-request-schema.json
slug: ec2-auto-scaling-scheduled-update-group-action-request
source_filename: ec2-auto-scaling-scheduled-update-group-action-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scheduled-update-group-action-request-schema.json\",\n  \"title\": \"ScheduledUpdateGroupActionRequest\",\n  \"description\": \"Describes information used for one or more scheduled scaling action updates in a <a>BatchPutScheduledUpdateGroupAction</a> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScheduledActionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the scaling action.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"<p>The date and time for the action to start, in YYYY-MM-DDThh:mm:ssZ\
  \ format in UTC/GMT only and in quotes (for example, <code>\\\"2019-06-01T00:00:00Z\\\"</code>).</p> <p>If you specify <code>Recurrence</code> and <code>StartTime</code>, Amazon EC2 Auto Scaling performs the action at this time, and then performs the action based on the specified recurrence.</p> <p>If you try to schedule the action in the past, Amazon EC2 Auto Scaling returns an error message.</p>\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"The date and time for the recurring schedule to end, in UTC.\"\n        }\n      ]\n    },\n    \"Recurrence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>The recurring schedule for the action, in Unix cron syntax format. This format consists of five fields separated by white spaces: [Minute]\
  \ [Hour] [Day_of_Month] [Month_of_Year] [Day_of_Week]. The value must be in quotes (for example, <code>\\\"30 0 1 1,6,12 *\\\"</code>). For more information about this format, see <a href=\\\"http://crontab.org\\\">Crontab</a>.</p> <p>When <code>StartTime</code> and <code>EndTime</code> are specified with <code>Recurrence</code>, they form the boundaries of when the recurring action starts and stops.</p> <p>Cron expressions use Universal Coordinated Time (UTC) by default.</p>\"\n        }\n      ]\n    },\n    \"MinSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupMinSize\"\n        },\n        {\n          \"description\": \"The minimum size of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"MaxSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupMaxSize\"\n        },\n        {\n          \"description\": \"The maximum size of the Auto Scaling group.\"\n        }\n      ]\n\
  \    },\n    \"DesiredCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupDesiredCapacity\"\n        },\n        {\n          \"description\": \"The desired capacity is the initial capacity of the Auto Scaling group after the scheduled action runs and the capacity it attempts to maintain.\"\n        }\n      ]\n    },\n    \"TimeZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>Specifies the time zone for a cron expression. If a time zone is not provided, UTC is used by default. </p> <p>Valid values are the canonical names of the IANA time zones, derived from the IANA Time Zone Database (such as <code>Etc/GMT+9</code> or <code>Pacific/Tahiti</code>). For more information, see <a href=\\\"https://en.wikipedia.org/wiki/List_of_tz_database_time_zones\\\">https://en.wikipedia.org/wiki/List_of_tz_database_time_zones</a>.</p>\"\n\
  \        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ScheduledActionName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scheduled-update-group-action-request-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: ScheduledUpdateGroupActionRequest
---
