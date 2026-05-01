---
description: InstanceStatus is deprecated, use TargetStatus instead.
layout: schema
name: InstanceStatus
properties_list: []
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-instance-status-schema.json
slug: amazon-codedeploy-instance-status
source_filename: amazon-codedeploy-instance-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-instance-status-schema.json\",\n  \"title\": \"InstanceStatus\",\n  \"description\": \"InstanceStatus is deprecated, use TargetStatus instead.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Pending\",\n    \"InProgress\",\n    \"Succeeded\",\n    \"Failed\",\n    \"Skipped\",\n    \"Unknown\",\n    \"Ready\"\n  ],\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-instance-status-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: InstanceStatus
---
