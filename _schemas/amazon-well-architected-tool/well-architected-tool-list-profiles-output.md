---
description: ListProfilesOutput schema from AWS Well-Architected Tool API
layout: schema
name: ListProfilesOutput
properties_list:
- description: ''
  name: ProfileSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-profiles-output-schema.json
slug: well-architected-tool-list-profiles-output
source_filename: well-architected-tool-list-profiles-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProfileSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileSummaries\"\n        },\n        {\n          \"description\": \"Profile summaries.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListProfilesOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-profiles-output-schema.json\",\n  \"description\": \"ListProfilesOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-profiles-output-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListProfilesOutput
---
