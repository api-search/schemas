---
description: Information about how to remediate a finding.
layout: schema
name: Remediation
properties_list:
- description: ''
  name: recommendation
  type: object
- description: ''
  name: suggestedFixes
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-remediation-schema.json
slug: amazon-codeguru-security-remediation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-remediation-schema.json\",\n  \"title\": \"Remediation\",\n  \"description\": \"Information about how to remediate a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recommendation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Recommendation\"\n        },\n        {\n          \"description\": \"An object that contains information about the recommended course of action to remediate a finding.\"\n        }\n      ]\n    },\n    \"suggestedFixes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SuggestedFixes\"\n        },\n        {\n          \"description\": \"A list of <code>SuggestedFix</code> objects. Each object contains information about a suggested code fix to remediate the finding.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-remediation-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: Remediation
---
