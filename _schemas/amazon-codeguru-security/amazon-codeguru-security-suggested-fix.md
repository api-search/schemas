---
description: Information about the suggested code fix to remediate a finding.
layout: schema
name: SuggestedFix
properties_list:
- description: ''
  name: code
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-suggested-fix-schema.json
slug: amazon-codeguru-security-suggested-fix
source_filename: amazon-codeguru-security-suggested-fix-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-suggested-fix-schema.json\",\n  \"title\": \"SuggestedFix\",\n  \"description\": \"Information about the suggested code fix to remediate a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The suggested code to add to your file. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A description of the suggested code fix and why it is being suggested. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-suggested-fix-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: SuggestedFix
---
