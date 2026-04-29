---
description: AmiNameString schema from EC2 Image Builder
layout: schema
name: AmiNameString
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-ami-name-string-schema.json
slug: ec2-image-builder-ami-name-string
source_filename: ec2-image-builder-ami-name-string-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-ami-name-string-schema.json\",\n  \"title\": \"AmiNameString\",\n  \"description\": \"AmiNameString schema from EC2 Image Builder\",\n  \"type\": \"string\",\n  \"pattern\": \"^[-_A-Za-z0-9{][-_A-Za-z0-9\\\\s:{}\\\\.]+[-_A-Za-z0-9}]$\",\n  \"minLength\": 1,\n  \"maxLength\": 127\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-ami-name-string-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: AmiNameString
---
