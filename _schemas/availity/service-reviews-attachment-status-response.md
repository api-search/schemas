---
description: AttachmentStatusResponse schema from Availity API
layout: schema
name: AttachmentStatusResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/service-reviews-attachment-status-response-schema.json
slug: service-reviews-attachment-status-response
source_filename: service-reviews-attachment-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-attachment-status-response-schema.json\",\n  \"title\": \"AttachmentStatusResponse\",\n  \"description\": \"AttachmentStatusResponse schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SUBMITTED\",\n        \"AV_ACCEPTED\",\n        \"AV_REJECTED\",\n        \"PY_ACCEPTED\",\n        \"PY_REJECTED\"\n      ],\n      \"example\": \"AV_ACCEPTED\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-attachment-status-response-schema.json
tags: []
title: AttachmentStatusResponse
---
