---
description: ImageStatus schema from EC2 Image Builder
layout: schema
name: ImageStatus
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-status-schema.json
slug: ec2-image-builder-image-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-status-schema.json\",\n  \"title\": \"ImageStatus\",\n  \"description\": \"ImageStatus schema from EC2 Image Builder\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PENDING\",\n    \"CREATING\",\n    \"BUILDING\",\n    \"TESTING\",\n    \"DISTRIBUTING\",\n    \"INTEGRATING\",\n    \"AVAILABLE\",\n    \"CANCELLED\",\n    \"FAILED\",\n    \"DEPRECATED\",\n    \"DELETED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-status-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageStatus
---
