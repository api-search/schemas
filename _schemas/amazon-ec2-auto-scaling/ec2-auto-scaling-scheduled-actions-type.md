---
description: ScheduledActionsType schema from Auto Scaling
layout: schema
name: ScheduledActionsType
properties_list:
- description: ''
  name: ScheduledUpdateGroupActions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-scheduled-actions-type-schema.json
slug: ec2-auto-scaling-scheduled-actions-type
source_filename: ec2-auto-scaling-scheduled-actions-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scheduled-actions-type-schema.json\",\n  \"title\": \"ScheduledActionsType\",\n  \"description\": \"ScheduledActionsType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScheduledUpdateGroupActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduledUpdateGroupActions\"\n        },\n        {\n          \"description\": \"The scheduled actions.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A string that indicates that the response contains more items than can be returned in a single response. To receive additional items, specify this string for the <code>NextToken</code>\
  \ value when requesting the next set of items. This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"ScheduledUpdateGroupActions\": [\n      {\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"DesiredCapacity\": 4,\n        \"MaxSize\": 6,\n        \"MinSize\": 2,\n        \"Recurrence\": \"30 0 1 12 0\",\n        \"ScheduledActionARN\": \"arn:aws:autoscaling:us-west-2:123456789012:scheduledUpdateGroupAction:8e86b655-b2e6-4410-8f29-b4f094d6871c:autoScalingGroupName/my-auto-scaling-group:scheduledActionName/my-scheduled-action\",\n        \"ScheduledActionName\": \"my-scheduled-action\",\n        \"StartTime\": \"2016-12-01T00:30:00+00:00\",\n        \"Time\": \"2016-12-01T00:30:00+00:00\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scheduled-actions-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: ScheduledActionsType
---
