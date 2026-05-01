---
description: Timezone schema from EC2 Image Builder
layout: schema
name: Timezone
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-timezone-schema.json
slug: ec2-image-builder-timezone
source_filename: ec2-image-builder-timezone-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-timezone-schema.json\",\n  \"title\": \"Timezone\",\n  \"description\": \"Timezone schema from EC2 Image Builder\",\n  \"type\": \"string\",\n  \"pattern\": \"[a-zA-Z0-9]{2,}(?:\\\\/[a-zA-z0-9-_+]+)*\",\n  \"minLength\": 3,\n  \"maxLength\": 100\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-timezone-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: Timezone
---
