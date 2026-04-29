---
description: GetLensOutput schema from AWS Well-Architected Tool API
layout: schema
name: GetLensOutput
properties_list:
- description: ''
  name: Lens
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-get-lens-output-schema.json
slug: well-architected-tool-get-lens-output
source_filename: well-architected-tool-get-lens-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Lens\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Lens\"\n        },\n        {\n          \"description\": \"A lens return object.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetLensOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-lens-output-schema.json\",\n  \"description\": \"GetLensOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-lens-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: GetLensOutput
---
