---
description: Contains vulnerability counts for a specific image pipeline.
layout: schema
name: ImagePipelineAggregation
properties_list:
- description: ''
  name: imagePipelineArn
  type: object
- description: ''
  name: severityCounts
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-pipeline-aggregation-schema.json
slug: ec2-image-builder-image-pipeline-aggregation
source_filename: ec2-image-builder-image-pipeline-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-pipeline-aggregation-schema.json\",\n  \"title\": \"ImagePipelineAggregation\",\n  \"description\": \"Contains vulnerability counts for a specific image pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imagePipelineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImagePipelineArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the image pipeline for this aggregation.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCounts\"\n        },\n        {\n          \"description\": \"Counts by severity level for medium severity and higher level findings, plus a total for all of the findings\
  \ for the specified image pipeline.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-pipeline-aggregation-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImagePipelineAggregation
---
