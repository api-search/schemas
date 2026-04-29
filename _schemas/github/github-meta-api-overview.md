---
description: Api Overview
layout: schema
name: api-overview
properties_list:
- description: ''
  name: verifiable_password_authentication
  type: boolean
- description: ''
  name: packages
  type: array
- description: ''
  name: dependabot
  type: array
- description: ''
  name: domains
  type: object
- description: ''
  name: installed_version
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-meta-api-overview-schema.json
slug: github-meta-api-overview
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-meta-api-overview-schema.json\",\n  \"title\": \"api-overview\",\n  \"description\": \"Api Overview\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"verifiable_password_authentication\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"packages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"192.0.2.1\"\n      ]\n    },\n    \"dependabot\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"192.0.2.1\"\n      ]\n    },\n    \"domains\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"website\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"example\"\
  : [\n              \"example.com\"\n            ]\n          }\n        },\n        \"codespaces\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"example\": [\n              \"example.com\"\n            ]\n          }\n        },\n        \"copilot\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"example\": [\n              \"example.com\"\n            ]\n          }\n        },\n        \"packages\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"example\": [\n              \"example.com\"\n            ]\n          }\n        },\n        \"actions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"example\": [\n              \"example.com\"\n            ]\n          }\n        }\n      }\n    },\n    \"installed_version\": {\n      \"type\": \"\
  string\",\n      \"example\": \"3.9.0\"\n    }\n  },\n  \"required\": [\n    \"verifiable_password_authentication\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-meta-api-overview-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: api-overview
---
