---
description: Contains vulnerability counts for a specific image.
layout: schema
name: ImageAggregation
properties_list:
- description: ''
  name: imageBuildVersionArn
  type: object
- description: ''
  name: severityCounts
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-aggregation-schema.json
slug: ec2-image-builder-image-aggregation
source_filename: ec2-image-builder-image-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-aggregation-schema.json\",\n  \"title\": \"ImageAggregation\",\n  \"description\": \"Contains vulnerability counts for a specific image.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imageBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the image for this aggregation.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCounts\"\n        },\n        {\n          \"description\": \"Counts by severity level for medium severity and higher level findings, plus a total for all of the findings for the specified image.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-aggregation-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageAggregation
---
