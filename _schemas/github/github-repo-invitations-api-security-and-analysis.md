---
description: security-and-analysis from GitHub API
layout: schema
name: security-and-analysis
properties_list:
- description: ''
  name: advanced_security
  type: object
- description: ''
  name: secret_scanning
  type: object
- description: ''
  name: secret_scanning_push_protection
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-invitations-api-security-and-analysis-schema.json
slug: github-repo-invitations-api-security-and-analysis
source_filename: github-repo-invitations-api-security-and-analysis-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-invitations-api-security-and-analysis-schema.json\",\n  \"title\": \"security-and-analysis\",\n  \"description\": \"security-and-analysis from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"advanced_security\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"enabled\",\n            \"disabled\"\n          ]\n        }\n      }\n    },\n    \"secret_scanning\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"enabled\",\n            \"disabled\"\n          ]\n        }\n      }\n    },\n    \"secret_scanning_push_protection\": {\n      \"type\": \"object\",\n      \"properties\": {\n\
  \        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"enabled\",\n            \"disabled\"\n          ]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-invitations-api-security-and-analysis-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: security-and-analysis
---
