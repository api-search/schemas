---
description: Includes counts by severity level for medium severity and higher level findings, plus a total for all of the findings for the specified filter.
layout: schema
name: SeverityCounts
properties_list:
- description: ''
  name: all
  type: object
- description: ''
  name: critical
  type: object
- description: ''
  name: high
  type: object
- description: ''
  name: medium
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-severity-counts-schema.json
slug: ec2-image-builder-severity-counts
source_filename: ec2-image-builder-severity-counts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-severity-counts-schema.json\",\n  \"title\": \"SeverityCounts\",\n  \"description\": \"Includes counts by severity level for medium severity and higher level findings, plus a total for all of the findings for the specified filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"all\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCountNumber\"\n        },\n        {\n          \"description\": \"The total number of findings across all severity levels for the specified filter.\"\n        }\n      ]\n    },\n    \"critical\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCountNumber\"\n        },\n        {\n          \"description\": \"The number of critical severity findings for the specified\
  \ filter.\"\n        }\n      ]\n    },\n    \"high\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCountNumber\"\n        },\n        {\n          \"description\": \"The number of high severity findings for the specified filter.\"\n        }\n      ]\n    },\n    \"medium\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCountNumber\"\n        },\n        {\n          \"description\": \"The number of medium severity findings for the specified filter.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-severity-counts-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: SeverityCounts
---
