---
description: CreateProfileOutput schema from AWS Well-Architected Tool API
layout: schema
name: CreateProfileOutput
properties_list:
- description: ''
  name: ProfileArn
  type: object
- description: ''
  name: ProfileVersion
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-create-profile-output-schema.json
slug: well-architected-tool-create-profile-output
source_filename: well-architected-tool-create-profile-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileArn\"\n        },\n        {\n          \"description\": \"The profile ARN.\"\n        }\n      ]\n    },\n    \"ProfileVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileVersion\"\n        },\n        {\n          \"description\": \"Version of the profile.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateProfileOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-profile-output-schema.json\",\n  \"description\": \"CreateProfileOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-profile-output-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CreateProfileOutput
---
