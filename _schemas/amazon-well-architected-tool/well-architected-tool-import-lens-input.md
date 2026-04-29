---
description: ImportLensInput schema from AWS Well-Architected Tool API
layout: schema
name: ImportLensInput
properties_list:
- description: ''
  name: LensAlias
  type: object
- description: ''
  name: JSONString
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-import-lens-input-schema.json
slug: well-architected-tool-import-lens-input
source_filename: well-architected-tool-import-lens-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"JSONString\",\n    \"ClientRequestToken\"\n  ],\n  \"title\": \"ImportLensInput\",\n  \"properties\": {\n    \"LensAlias\": {\n      \"$ref\": \"#/components/schemas/LensAlias\"\n    },\n    \"JSONString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensJSON\"\n        },\n        {\n          \"description\": \"The JSON representation of a lens.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"$ref\": \"#/components/schemas/ClientRequestToken\"\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags to associate to a lens.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-import-lens-input-schema.json\"\
  ,\n  \"description\": \"ImportLensInput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-import-lens-input-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ImportLensInput
---
