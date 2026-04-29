---
description: ProcessesType schema from Auto Scaling
layout: schema
name: ProcessesType
properties_list:
- description: ''
  name: Processes
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-processes-type-schema.json
slug: ec2-auto-scaling-processes-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-processes-type-schema.json\",\n  \"title\": \"ProcessesType\",\n  \"description\": \"ProcessesType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Processes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Processes\"\n        },\n        {\n          \"description\": \"The names of the process types.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"Processes\": [\n      {\n        \"ProcessName\": \"AZRebalance\"\n      },\n      {\n        \"ProcessName\": \"AddToLoadBalancer\"\n      },\n      {\n        \"ProcessName\": \"AlarmNotification\"\n      },\n      {\n        \"ProcessName\": \"HealthCheck\"\n      },\n      {\n        \"ProcessName\": \"Launch\"\n      },\n      {\n        \"ProcessName\"\
  : \"ReplaceUnhealthy\"\n      },\n      {\n        \"ProcessName\": \"ScheduledActions\"\n      },\n      {\n        \"ProcessName\": \"Terminate\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-processes-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: ProcessesType
---
