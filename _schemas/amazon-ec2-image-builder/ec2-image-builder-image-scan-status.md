---
description: ImageScanStatus schema from EC2 Image Builder
layout: schema
name: ImageScanStatus
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-scan-status-schema.json
slug: ec2-image-builder-image-scan-status
source_filename: ec2-image-builder-image-scan-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-status-schema.json\",\n  \"title\": \"ImageScanStatus\",\n  \"description\": \"ImageScanStatus schema from EC2 Image Builder\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PENDING\",\n    \"SCANNING\",\n    \"COLLECTING\",\n    \"COMPLETED\",\n    \"ABANDONED\",\n    \"FAILED\",\n    \"TIMED_OUT\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-status-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageScanStatus
---
