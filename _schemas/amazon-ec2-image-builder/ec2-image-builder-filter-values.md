---
description: FilterValues schema from EC2 Image Builder
layout: schema
name: FilterValues
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-filter-values-schema.json
slug: ec2-image-builder-filter-values
source_filename: ec2-image-builder-filter-values-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-filter-values-schema.json\",\n  \"title\": \"FilterValues\",\n  \"description\": \"FilterValues schema from EC2 Image Builder\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/FilterValue\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 10\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-filter-values-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: FilterValues
---
