---
description: ScalingProcessQuery schema from Auto Scaling
layout: schema
name: ScalingProcessQuery
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: ScalingProcesses
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-scaling-process-query-schema.json
slug: ec2-auto-scaling-scaling-process-query
source_filename: ec2-auto-scaling-scaling-process-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scaling-process-query-schema.json\",\n  \"title\": \"ScalingProcessQuery\",\n  \"description\": \"ScalingProcessQuery schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"ScalingProcesses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProcessNames\"\n        },\n        {\n          \"description\": \"<p>One or more of the following processes:</p> <ul> <li> <p> <code>Launch</code> </p> </li> <li> <p> <code>Terminate</code> </p> </li> <li> <p> <code>AddToLoadBalancer</code> </p>\
  \ </li> <li> <p> <code>AlarmNotification</code> </p> </li> <li> <p> <code>AZRebalance</code> </p> </li> <li> <p> <code>HealthCheck</code> </p> </li> <li> <p> <code>InstanceRefresh</code> </p> </li> <li> <p> <code>ReplaceUnhealthy</code> </p> </li> <li> <p> <code>ScheduledActions</code> </p> </li> </ul> <p>If you omit this property, all processes are specified.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scaling-process-query-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: ScalingProcessQuery
---
