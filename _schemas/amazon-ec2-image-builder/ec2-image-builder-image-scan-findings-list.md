---
description: ImageScanFindingsList schema from EC2 Image Builder
layout: schema
name: ImageScanFindingsList
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-scan-findings-list-schema.json
slug: ec2-image-builder-image-scan-findings-list
source_filename: ec2-image-builder-image-scan-findings-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-findings-list-schema.json\",\n  \"title\": \"ImageScanFindingsList\",\n  \"description\": \"ImageScanFindingsList schema from EC2 Image Builder\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ImageScanFinding\"\n  },\n  \"maxItems\": 25\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-findings-list-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageScanFindingsList
---
