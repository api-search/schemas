---
description: Describes whether detailed monitoring is enabled for the Auto Scaling instances.
layout: schema
name: InstanceMonitoring
properties_list:
- description: ''
  name: Enabled
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-instance-monitoring-schema.json
slug: ec2-auto-scaling-instance-monitoring
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-monitoring-schema.json\",\n  \"title\": \"InstanceMonitoring\",\n  \"description\": \"Describes whether detailed monitoring is enabled for the Auto Scaling instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MonitoringEnabled\"\n        },\n        {\n          \"description\": \"If <code>true</code>, detailed monitoring is enabled. Otherwise, basic monitoring is enabled.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-monitoring-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: InstanceMonitoring
---
