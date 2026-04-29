---
description: ImageList schema from Aqua Security API
layout: schema
name: ImageList
properties_list:
- description: Total number of images
  name: count
  type: integer
- description: ''
  name: result
  type: array
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-image-list-schema.json
slug: aqua-security-api-image-list
source_filename: aqua-security-api-image-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"example\": 100,\n      \"description\": \"Total number of images\"\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"registry\": {\n            \"type\": \"string\",\n            \"example\": \"docker-hub\",\n            \"description\": \"Name of the container registry\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"nginx\",\n            \"description\": \"Image repository name\"\n          },\n          \"tag\": {\n            \"type\": \"string\",\n            \"example\": \"latest\",\n            \"description\": \"Image tag\"\n          },\n          \"digest\": {\n            \"type\": \"string\",\n            \"example\": \"sha256:a1b2c3d4e5f6a1b2c3d4e5f6a1b2c3d4e5f6a1b2c3d4e5f6a1b2c3d4e5f6a1b2\",\n            \"description\"\
  : \"Image content digest (SHA256)\"\n          },\n          \"scan_status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"pending\",\n              \"in-progress\",\n              \"completed\",\n              \"failed\"\n            ],\n            \"example\": \"completed\",\n            \"description\": \"Current scan status\"\n          },\n          \"vulnerabilities\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"critical\": {},\n              \"high\": {},\n              \"medium\": {},\n              \"low\": {},\n              \"negligible\": {}\n            }\n          },\n          \"disallowed\": {\n            \"type\": \"boolean\",\n            \"example\": false,\n            \"description\": \"Whether the image is blocked by policy\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-image-list-schema.json\"\
  ,\n  \"title\": \"ImageList\",\n  \"description\": \"ImageList schema from Aqua Security API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-image-list-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: ImageList
---
