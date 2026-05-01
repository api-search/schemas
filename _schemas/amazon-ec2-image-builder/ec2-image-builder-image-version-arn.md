---
description: ImageVersionArn schema from EC2 Image Builder
layout: schema
name: ImageVersionArn
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-version-arn-schema.json
slug: ec2-image-builder-image-version-arn
source_filename: ec2-image-builder-image-version-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-version-arn-schema.json\",\n  \"title\": \"ImageVersionArn\",\n  \"description\": \"ImageVersionArn schema from EC2 Image Builder\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws[^:]*:imagebuilder:[^:]+:(?:[0-9]{12}|aws):image/[a-z0-9-_]+/[0-9]+\\\\.[0-9]+\\\\.[0-9]+$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-version-arn-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageVersionArn
---
