---
description: Input to disassociate lens reviews.
layout: schema
name: DisassociateLensesInput
properties_list:
- description: ''
  name: LensAliases
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-disassociate-lenses-input-schema.json
slug: well-architected-tool-disassociate-lenses-input
source_filename: well-architected-tool-disassociate-lenses-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"LensAliases\"\n  ],\n  \"title\": \"DisassociateLensesInput\",\n  \"properties\": {\n    \"LensAliases\": {\n      \"$ref\": \"#/components/schemas/LensAliases\"\n    }\n  },\n  \"description\": \"Input to disassociate lens reviews.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-disassociate-lenses-input-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-disassociate-lenses-input-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: DisassociateLensesInput
---
