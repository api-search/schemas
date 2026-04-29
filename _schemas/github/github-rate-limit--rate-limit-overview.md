---
description: Rate Limit Overview
layout: schema
name: rate-limit-overview
properties_list:
- description: ''
  name: resources
  type: object
- description: ''
  name: rate
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-rate-limit--rate-limit-overview-schema.json
slug: github-rate-limit--rate-limit-overview
source_filename: github-rate-limit--rate-limit-overview-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-rate-limit--rate-limit-overview-schema.json\",\n  \"title\": \"rate-limit-overview\",\n  \"description\": \"Rate Limit Overview\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resources\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"core\": {\n          \"$ref\": \"#/components/schemas/rate-limit\"\n        },\n        \"graphql\": {\n          \"$ref\": \"#/components/schemas/rate-limit\"\n        },\n        \"search\": {\n          \"$ref\": \"#/components/schemas/rate-limit\"\n        },\n        \"code_search\": {\n          \"$ref\": \"#/components/schemas/rate-limit\"\n        },\n        \"source_import\": {\n          \"$ref\": \"#/components/schemas/rate-limit\"\n        },\n        \"integration_manifest\": {\n          \"$ref\": \"#/components/schemas/rate-limit\"\
  \n        },\n        \"code_scanning_upload\": {\n          \"$ref\": \"#/components/schemas/rate-limit\"\n        },\n        \"actions_runner_registration\": {\n          \"$ref\": \"#/components/schemas/rate-limit\"\n        },\n        \"scim\": {\n          \"$ref\": \"#/components/schemas/rate-limit\"\n        }\n      },\n      \"required\": [\n        \"core\",\n        \"search\"\n      ]\n    },\n    \"rate\": {\n      \"$ref\": \"#/components/schemas/rate-limit\"\n    }\n  },\n  \"required\": [\n    \"rate\",\n    \"resources\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-rate-limit--rate-limit-overview-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: rate-limit-overview
---
