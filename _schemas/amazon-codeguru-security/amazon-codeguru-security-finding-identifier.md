---
description: An object that contains information about a finding and the scan that generated it.
layout: schema
name: FindingIdentifier
properties_list:
- description: ''
  name: findingId
  type: object
- description: ''
  name: scanName
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-finding-identifier-schema.json
slug: amazon-codeguru-security-finding-identifier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-finding-identifier-schema.json\",\n  \"title\": \"FindingIdentifier\",\n  \"description\": \"An object that contains information about a finding and the scan that generated it. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier for a finding.\"\n        }\n      ]\n    },\n    \"scanName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the scan that generated the finding. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"findingId\",\n    \"scanName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-finding-identifier-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: FindingIdentifier
---
