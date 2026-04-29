---
description: Output of a list lenses call.
layout: schema
name: ListLensesOutput
properties_list:
- description: ''
  name: LensSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-lenses-output-schema.json
slug: well-architected-tool-list-lenses-output
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LensSummaries\": {\n      \"$ref\": \"#/components/schemas/LensSummaries\"\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    }\n  },\n  \"description\": \"Output of a list lenses call.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListLensesOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-lenses-output-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-lenses-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListLensesOutput
---
