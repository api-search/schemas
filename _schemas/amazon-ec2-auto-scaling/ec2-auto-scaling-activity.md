---
description: Describes scaling activity, which is a long-running process that represents a change to your Auto Scaling group, such as changing its size or replacing an instance.
layout: schema
name: Activity
properties_list:
- description: ''
  name: ActivityId
  type: object
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Cause
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: StatusCode
  type: object
- description: ''
  name: StatusMessage
  type: object
- description: ''
  name: Progress
  type: object
- description: ''
  name: Details
  type: object
- description: ''
  name: AutoScalingGroupState
  type: object
- description: ''
  name: AutoScalingGroupARN
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-activity-schema.json
slug: ec2-auto-scaling-activity
source_filename: ec2-auto-scaling-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-activity-schema.json\",\n  \"title\": \"Activity\",\n  \"description\": \"Describes scaling activity, which is a long-running process that represents a change to your Auto Scaling group, such as changing its size or replacing an instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActivityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"The ID of the activity.\"\n        }\n      ]\n    },\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A friendly, more verbose description of the activity.\"\n        }\n      ]\n    },\n    \"Cause\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen1023\"\n        },\n        {\n          \"description\": \"The reason the activity began.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"The start time of the activity.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"The end time of the activity.\"\n        }\n      ]\n    },\n    \"StatusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScalingActivityStatusCode\"\
  \n        },\n        {\n          \"description\": \"The current status of the activity.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"A friendly, more verbose description of the activity status.\"\n        }\n      ]\n    },\n    \"Progress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Progress\"\n        },\n        {\n          \"description\": \"A value between 0 and 100 that indicates the progress of the activity.\"\n        }\n      ]\n    },\n    \"Details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"The details about the activity.\"\n        }\n      ]\n    },\n    \"AutoScalingGroupState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupState\"\
  \n        },\n        {\n          \"description\": \"The state of the Auto Scaling group, which is either <code>InService</code> or <code>Deleted</code>.\"\n        }\n      ]\n    },\n    \"AutoScalingGroupARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Auto Scaling group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ActivityId\",\n    \"AutoScalingGroupName\",\n    \"Cause\",\n    \"StartTime\",\n    \"StatusCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-activity-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: Activity
---
