---
description: <p>List of lens aliases to associate or disassociate with a workload. Up to 10 lenses can be specified.</p> <p>Identify a lens using its <a>LensSummary$LensAlias</a>.</p>
layout: schema
name: LensAliases
properties_list: []
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-lens-aliases-schema.json
slug: well-architected-tool-lens-aliases
source_json: "{\n  \"type\": \"array\",\n  \"description\": \"<p>List of lens aliases to associate or disassociate with a workload. Up to 10 lenses can be specified.</p> <p>Identify a lens using its <a>LensSummary$LensAlias</a>.</p>\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/LensAlias\"\n  },\n  \"minItems\": 1,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LensAliases\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-aliases-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-aliases-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: LensAliases
---
