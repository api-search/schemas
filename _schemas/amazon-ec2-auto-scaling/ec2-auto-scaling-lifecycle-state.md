---
description: LifecycleState schema from Auto Scaling
layout: schema
name: LifecycleState
properties_list: []
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-lifecycle-state-schema.json
slug: ec2-auto-scaling-lifecycle-state
source_filename: ec2-auto-scaling-lifecycle-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-lifecycle-state-schema.json\",\n  \"title\": \"LifecycleState\",\n  \"description\": \"LifecycleState schema from Auto Scaling\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Pending\",\n    \"Pending:Wait\",\n    \"Pending:Proceed\",\n    \"Quarantined\",\n    \"InService\",\n    \"Terminating\",\n    \"Terminating:Wait\",\n    \"Terminating:Proceed\",\n    \"Terminated\",\n    \"Detaching\",\n    \"Detached\",\n    \"EnteringStandby\",\n    \"Standby\",\n    \"Warmed:Pending\",\n    \"Warmed:Pending:Wait\",\n    \"Warmed:Pending:Proceed\",\n    \"Warmed:Terminating\",\n    \"Warmed:Terminating:Wait\",\n    \"Warmed:Terminating:Proceed\",\n    \"Warmed:Terminated\",\n    \"Warmed:Stopped\",\n    \"Warmed:Running\",\n    \"Warmed:Hibernated\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-lifecycle-state-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: LifecycleState
---
