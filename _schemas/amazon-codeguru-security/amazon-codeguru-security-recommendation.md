---
description: Information about the recommended course of action to remediate a finding.
layout: schema
name: Recommendation
properties_list:
- description: ''
  name: text
  type: object
- description: ''
  name: url
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-recommendation-schema.json
slug: amazon-codeguru-security-recommendation
source_filename: amazon-codeguru-security-recommendation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-recommendation-schema.json\",\n  \"title\": \"Recommendation\",\n  \"description\": \"Information about the recommended course of action to remediate a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The recommended course of action to remediate the finding.\"\n        }\n      ]\n    },\n    \"url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The URL address to the recommendation for remediating the finding. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-recommendation-schema.json
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: Recommendation
---
