---
description: ImportLensOutput schema from AWS Well-Architected Tool API
layout: schema
name: ImportLensOutput
properties_list:
- description: ''
  name: LensArn
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-import-lens-output-schema.json
slug: well-architected-tool-import-lens-output
source_filename: well-architected-tool-import-lens-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"The ARN for the lens that was created or updated.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportLensStatus\"\n        },\n        {\n          \"description\": \"The status of the imported lens.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImportLensOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-import-lens-output-schema.json\",\n  \"description\": \"ImportLensOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-import-lens-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ImportLensOutput
---
