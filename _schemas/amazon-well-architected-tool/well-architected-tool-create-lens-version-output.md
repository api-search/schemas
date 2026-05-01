---
description: CreateLensVersionOutput schema from AWS Well-Architected Tool API
layout: schema
name: CreateLensVersionOutput
properties_list:
- description: ''
  name: LensArn
  type: object
- description: ''
  name: LensVersion
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-create-lens-version-output-schema.json
slug: well-architected-tool-create-lens-version-output
source_filename: well-architected-tool-create-lens-version-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"The ARN for the lens.\"\n        }\n      ]\n    },\n    \"LensVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensVersion\"\n        },\n        {\n          \"description\": \"The version of the lens.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateLensVersionOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-lens-version-output-schema.json\",\n  \"description\": \"CreateLensVersionOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-lens-version-output-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CreateLensVersionOutput
---
