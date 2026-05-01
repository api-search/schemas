---
description: OrganizationalUnitArnList schema from EC2 Image Builder
layout: schema
name: OrganizationalUnitArnList
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-organizational-unit-arn-list-schema.json
slug: ec2-image-builder-organizational-unit-arn-list
source_filename: ec2-image-builder-organizational-unit-arn-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-organizational-unit-arn-list-schema.json\",\n  \"title\": \"OrganizationalUnitArnList\",\n  \"description\": \"OrganizationalUnitArnList schema from EC2 Image Builder\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/OrganizationalUnitArn\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 25\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-organizational-unit-arn-list-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: OrganizationalUnitArnList
---
