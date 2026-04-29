---
description: The differences between the base and latest versions of the lens.
layout: schema
name: VersionDifferences
properties_list:
- description: ''
  name: PillarDifferences
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-version-differences-schema.json
slug: well-architected-tool-version-differences
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"PillarDifferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PillarDifferences\"\n        },\n        {\n          \"description\": \"The differences between the base and latest versions of the lens.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The differences between the base and latest versions of the lens.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VersionDifferences\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-version-differences-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-version-differences-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: VersionDifferences
---
