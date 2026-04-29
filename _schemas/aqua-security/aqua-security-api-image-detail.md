---
description: ImageDetail schema from Aqua Security API
layout: schema
name: ImageDetail
properties_list:
- description: Name of the container registry
  name: registry
  type: string
- description: Image repository name
  name: name
  type: string
- description: Image tag
  name: tag
  type: string
- description: Image content digest (SHA256)
  name: digest
  type: string
- description: Current scan status
  name: scan_status
  type: string
- description: ''
  name: vulnerabilities
  type: object
- description: Whether the image is blocked by policy
  name: disallowed
  type: boolean
- description: Operating system of the image
  name: os
  type: string
- description: Image size in bytes
  name: size
  type: integer
- description: Image creation timestamp
  name: created
  type: string
- description: Date the image was last scanned
  name: scan_date
  type: string
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-image-detail-schema.json
slug: aqua-security-api-image-detail
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"registry\": {\n      \"type\": \"string\",\n      \"example\": \"docker-hub\",\n      \"description\": \"Name of the container registry\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"nginx\",\n      \"description\": \"Image repository name\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"example\": \"latest\",\n      \"description\": \"Image tag\"\n    },\n    \"digest\": {\n      \"type\": \"string\",\n      \"example\": \"sha256:a1b2c3d4e5f6a1b2c3d4e5f6a1b2c3d4e5f6a1b2c3d4e5f6a1b2c3d4e5f6a1b2\",\n      \"description\": \"Image content digest (SHA256)\"\n    },\n    \"scan_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"in-progress\",\n        \"completed\",\n        \"failed\"\n      ],\n      \"example\": \"completed\",\n      \"description\": \"Current scan status\"\n    },\n    \"vulnerabilities\": {\n      \"type\": \"object\"\
  ,\n      \"properties\": {\n        \"critical\": {\n          \"type\": \"integer\",\n          \"example\": 0,\n          \"description\": \"Number of critical severity vulnerabilities\"\n        },\n        \"high\": {\n          \"type\": \"integer\",\n          \"example\": 3,\n          \"description\": \"Number of high severity vulnerabilities\"\n        },\n        \"medium\": {\n          \"type\": \"integer\",\n          \"example\": 12,\n          \"description\": \"Number of medium severity vulnerabilities\"\n        },\n        \"low\": {\n          \"type\": \"integer\",\n          \"example\": 24,\n          \"description\": \"Number of low severity vulnerabilities\"\n        },\n        \"negligible\": {\n          \"type\": \"integer\",\n          \"example\": 5,\n          \"description\": \"Number of negligible severity vulnerabilities\"\n        }\n      }\n    },\n    \"disallowed\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\"\
  : \"Whether the image is blocked by policy\"\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"example\": \"debian:bullseye-slim\",\n      \"description\": \"Operating system of the image\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"example\": 142000000,\n      \"description\": \"Image size in bytes\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\",\n      \"description\": \"Image creation timestamp\"\n    },\n    \"scan_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:00:00Z\",\n      \"description\": \"Date the image was last scanned\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-image-detail-schema.json\",\n  \"title\": \"ImageDetail\",\n  \"description\"\
  : \"ImageDetail schema from Aqua Security API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-image-detail-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: ImageDetail
---
