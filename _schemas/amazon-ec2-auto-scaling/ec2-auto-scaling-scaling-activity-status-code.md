---
description: ScalingActivityStatusCode schema from Auto Scaling
layout: schema
name: ScalingActivityStatusCode
properties_list: []
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-scaling-activity-status-code-schema.json
slug: ec2-auto-scaling-scaling-activity-status-code
source_filename: ec2-auto-scaling-scaling-activity-status-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scaling-activity-status-code-schema.json\",\n  \"title\": \"ScalingActivityStatusCode\",\n  \"description\": \"ScalingActivityStatusCode schema from Auto Scaling\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PendingSpotBidPlacement\",\n    \"WaitingForSpotInstanceRequestId\",\n    \"WaitingForSpotInstanceId\",\n    \"WaitingForInstanceId\",\n    \"PreInService\",\n    \"InProgress\",\n    \"WaitingForELBConnectionDraining\",\n    \"MidLifecycleAction\",\n    \"WaitingForInstanceWarmup\",\n    \"Successful\",\n    \"Failed\",\n    \"Cancelled\",\n    \"WaitingForConnectionDraining\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-scaling-activity-status-code-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: ScalingActivityStatusCode
---
