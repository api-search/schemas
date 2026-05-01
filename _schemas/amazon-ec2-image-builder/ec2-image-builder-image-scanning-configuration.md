---
description: Contains settings for Image Builder image resource and container image scans.
layout: schema
name: ImageScanningConfiguration
properties_list:
- description: ''
  name: imageScanningEnabled
  type: object
- description: ''
  name: ecrConfiguration
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-scanning-configuration-schema.json
slug: ec2-image-builder-image-scanning-configuration
source_filename: ec2-image-builder-image-scanning-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scanning-configuration-schema.json\",\n  \"title\": \"ImageScanningConfiguration\",\n  \"description\": \"Contains settings for Image Builder image resource and container image scans.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imageScanningEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"A setting that indicates whether Image Builder keeps a snapshot of the vulnerability scans that Amazon Inspector runs against the build instance when you create a new image.\"\n        }\n      ]\n    },\n    \"ecrConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcrConfiguration\"\n        },\n        {\n          \"description\"\
  : \"Contains Amazon ECR settings for vulnerability scans.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scanning-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageScanningConfiguration
---
