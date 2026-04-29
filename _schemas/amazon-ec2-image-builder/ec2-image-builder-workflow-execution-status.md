---
description: WorkflowExecutionStatus schema from EC2 Image Builder
layout: schema
name: WorkflowExecutionStatus
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-workflow-execution-status-schema.json
slug: ec2-image-builder-workflow-execution-status
source_filename: ec2-image-builder-workflow-execution-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-workflow-execution-status-schema.json\",\n  \"title\": \"WorkflowExecutionStatus\",\n  \"description\": \"WorkflowExecutionStatus schema from EC2 Image Builder\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PENDING\",\n    \"SKIPPED\",\n    \"RUNNING\",\n    \"COMPLETED\",\n    \"FAILED\",\n    \"ROLLBACK_IN_PROGRESS\",\n    \"ROLLBACK_COMPLETED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-workflow-execution-status-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: WorkflowExecutionStatus
---
