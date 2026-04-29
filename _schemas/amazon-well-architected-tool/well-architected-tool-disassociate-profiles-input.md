---
description: DisassociateProfilesInput schema from AWS Well-Architected Tool API
layout: schema
name: DisassociateProfilesInput
properties_list:
- description: ''
  name: ProfileArns
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-disassociate-profiles-input-schema.json
slug: well-architected-tool-disassociate-profiles-input
source_filename: well-architected-tool-disassociate-profiles-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ProfileArns\"\n  ],\n  \"title\": \"DisassociateProfilesInput\",\n  \"properties\": {\n    \"ProfileArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProfileArns\"\n        },\n        {\n          \"description\": \"The list of profile ARNs to disassociate from the workload.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-disassociate-profiles-input-schema.json\",\n  \"description\": \"DisassociateProfilesInput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-disassociate-profiles-input-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: DisassociateProfilesInput
---
