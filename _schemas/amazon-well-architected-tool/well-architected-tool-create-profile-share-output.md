---
description: CreateProfileShareOutput schema from AWS Well-Architected Tool API
layout: schema
name: CreateProfileShareOutput
properties_list:
- description: ''
  name: ShareId
  type: object
- description: ''
  name: ProfileArn
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-create-profile-share-output-schema.json
slug: well-architected-tool-create-profile-share-output
source_filename: well-architected-tool-create-profile-share-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ShareId\": {\n      \"$ref\": \"#/components/schemas/ShareId\"\n    },\n    \"ProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileArn\"\n        },\n        {\n          \"description\": \"The profile ARN.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateProfileShareOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-profile-share-output-schema.json\",\n  \"description\": \"CreateProfileShareOutput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-create-profile-share-output-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: CreateProfileShareOutput
---
