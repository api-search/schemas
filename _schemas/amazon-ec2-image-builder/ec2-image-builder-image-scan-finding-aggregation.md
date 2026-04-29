---
description: This returns exactly one type of aggregation, based on the filter that Image Builder applies in its API action.
layout: schema
name: ImageScanFindingAggregation
properties_list:
- description: ''
  name: accountAggregation
  type: object
- description: ''
  name: imageAggregation
  type: object
- description: ''
  name: imagePipelineAggregation
  type: object
- description: ''
  name: vulnerabilityIdAggregation
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-scan-finding-aggregation-schema.json
slug: ec2-image-builder-image-scan-finding-aggregation
source_filename: ec2-image-builder-image-scan-finding-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-finding-aggregation-schema.json\",\n  \"title\": \"ImageScanFindingAggregation\",\n  \"description\": \"This returns exactly one type of aggregation, based on the filter that Image Builder applies in its API action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAggregation\"\n        },\n        {\n          \"description\": \"Returns an object that contains severity counts based on an account ID.\"\n        }\n      ]\n    },\n    \"imageAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageAggregation\"\n        },\n        {\n          \"description\": \"Returns an object that contains severity counts based\
  \ on the Amazon Resource Name (ARN) for a specific image.\"\n        }\n      ]\n    },\n    \"imagePipelineAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImagePipelineAggregation\"\n        },\n        {\n          \"description\": \"Returns an object that contains severity counts based on an image pipeline ARN.\"\n        }\n      ]\n    },\n    \"vulnerabilityIdAggregation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VulnerabilityIdAggregation\"\n        },\n        {\n          \"description\": \"Returns an object that contains severity counts based on vulnerability ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-scan-finding-aggregation-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageScanFindingAggregation
---
