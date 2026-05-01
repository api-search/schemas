---
description: WorkflowBuildVersionArn schema from EC2 Image Builder
layout: schema
name: WorkflowBuildVersionArn
properties_list: []
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-workflow-build-version-arn-schema.json
slug: ec2-image-builder-workflow-build-version-arn
source_filename: ec2-image-builder-workflow-build-version-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-workflow-build-version-arn-schema.json\",\n  \"title\": \"WorkflowBuildVersionArn\",\n  \"description\": \"WorkflowBuildVersionArn schema from EC2 Image Builder\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws(?:-[a-z]+)*:imagebuilder:[a-z]{2,}(?:-[a-z]+)+-[0-9]+:(?:[0-9]{12}|aws):workflow/(build|test|distribution)/[a-z0-9-_]+/[0-9]+\\\\.[0-9]+\\\\.[0-9]+/[0-9]+$\",\n  \"maxLength\": 1024\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-workflow-build-version-arn-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: WorkflowBuildVersionArn
---
