---
description: ImageRequest schema from Aqua Security API
layout: schema
name: ImageRequest
properties_list:
- description: Name of the configured registry
  name: registry
  type: string
- description: Full image name including tag
  name: image
  type: string
provider_name: Aqua Security
provider_slug: aqua-security
schema_file: json-schema/aqua-security-api-image-request-schema.json
slug: aqua-security-api-image-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"registry\": {\n      \"type\": \"string\",\n      \"example\": \"docker-hub\",\n      \"description\": \"Name of the configured registry\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"example\": \"nginx:latest\",\n      \"description\": \"Full image name including tag\"\n    }\n  },\n  \"required\": [\n    \"registry\",\n    \"image\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-image-request-schema.json\",\n  \"title\": \"ImageRequest\",\n  \"description\": \"ImageRequest schema from Aqua Security API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aqua-security/refs/heads/main/json-schema/aqua-security-api-image-request-schema.json
tags:
- Cloud Native
- Containers
- Kubernetes
- Runtime Protection
- Security
- Vulnerability Scanning
title: ImageRequest
---
