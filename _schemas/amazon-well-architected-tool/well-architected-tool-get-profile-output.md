---
description: GetProfileOutput schema from AWS Well-Architected Tool API
layout: schema
name: GetProfileOutput
properties_list:
- description: ''
  name: Profile
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-get-profile-output-schema.json
slug: well-architected-tool-get-profile-output
source_filename: well-architected-tool-get-profile-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Profile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Profile\"\n        },\n        {\n          \"description\": \"The profile.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetProfileOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-profile-output-schema.json\",\n  \"description\": \"GetProfileOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-get-profile-output-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: GetProfileOutput
---
