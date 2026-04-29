---
description: ExportLensOutput schema from AWS Well-Architected Tool API
layout: schema
name: ExportLensOutput
properties_list:
- description: ''
  name: LensJSON
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-export-lens-output-schema.json
slug: well-architected-tool-export-lens-output
source_filename: well-architected-tool-export-lens-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LensJSON\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensJSON\"\n        },\n        {\n          \"description\": \"The JSON representation of a lens.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExportLensOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-export-lens-output-schema.json\",\n  \"description\": \"ExportLensOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-export-lens-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ExportLensOutput
---
