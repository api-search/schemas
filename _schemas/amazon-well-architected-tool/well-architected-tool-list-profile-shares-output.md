---
description: ListProfileSharesOutput schema from AWS Well-Architected Tool API
layout: schema
name: ListProfileSharesOutput
properties_list:
- description: ''
  name: ProfileShareSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-profile-shares-output-schema.json
slug: well-architected-tool-list-profile-shares-output
source_filename: well-architected-tool-list-profile-shares-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProfileShareSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileShareSummaries\"\n        },\n        {\n          \"description\": \"Profile share summaries.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListProfileSharesOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-profile-shares-output-schema.json\",\n  \"description\": \"ListProfileSharesOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-profile-shares-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListProfileSharesOutput
---
