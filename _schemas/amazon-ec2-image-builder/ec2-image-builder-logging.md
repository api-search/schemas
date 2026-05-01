---
description: Logging configuration defines where Image Builder uploads your logs.
layout: schema
name: Logging
properties_list:
- description: ''
  name: s3Logs
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-logging-schema.json
slug: ec2-image-builder-logging
source_filename: ec2-image-builder-logging-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-logging-schema.json\",\n  \"title\": \"Logging\",\n  \"description\": \"Logging configuration defines where Image Builder uploads your logs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s3Logs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Logs\"\n        },\n        {\n          \"description\": \"The Amazon S3 logging configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-logging-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: Logging
---
