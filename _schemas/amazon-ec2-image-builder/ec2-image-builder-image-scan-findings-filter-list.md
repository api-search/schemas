---
description: ImageScanFindingsFilterList schema from EC2 Image Builder
layout: schema
name: ImageScanFindingsFilterList
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-scan-findings-filter-list-schema.json
slug: ec2-image-builder-image-scan-findings-filter-list
source_filename: ec2-image-builder-image-scan-findings-filter-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-findings-filter-list-schema.json\",\n  \"title\": \"ImageScanFindingsFilterList\",\n  \"description\": \"ImageScanFindingsFilterList schema from EC2 Image Builder\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ImageScanFindingsFilter\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 1\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-findings-filter-list-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageScanFindingsFilterList
---
