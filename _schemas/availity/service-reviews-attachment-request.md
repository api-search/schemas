---
description: AttachmentRequest schema from Availity API
layout: schema
name: AttachmentRequest
properties_list:
- description: ''
  name: payerId
  type: string
- description: ''
  name: patient
  type: object
- description: ''
  name: subscriber
  type: object
- description: ''
  name: provider
  type: object
- description: ''
  name: certificationNumber
  type: string
- description: ''
  name: attachments
  type: array
provider_name: availity
provider_slug: availity
schema_file: json-schema/service-reviews-attachment-request-schema.json
slug: service-reviews-attachment-request
source_filename: service-reviews-attachment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-attachment-request-schema.json\",\n  \"title\": \"AttachmentRequest\",\n  \"description\": \"AttachmentRequest schema from Availity API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"payerId\",\n    \"patient\",\n    \"subscriber\",\n    \"provider\",\n    \"certificationNumber\",\n    \"attachments\"\n  ],\n  \"properties\": {\n    \"payerId\": {\n      \"type\": \"string\",\n      \"example\": \"BCBS001\"\n    },\n    \"patient\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"Jane\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"Smith\"\n        }\n      }\n    },\n    \"subscriber\": {\n      \"type\": \"object\",\n      \"properties\": {\n \
  \       \"memberId\": {\n          \"type\": \"string\",\n          \"example\": \"MEM123456\"\n        }\n      }\n    },\n    \"provider\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"npi\": {\n          \"type\": \"string\",\n          \"example\": \"1234567890\"\n        }\n      }\n    },\n    \"certificationNumber\": {\n      \"type\": \"string\",\n      \"example\": \"AUTH-2025-001234\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"contentType\": {\n            \"type\": \"string\",\n            \"example\": \"application/pdf\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"example\": \"Clinical Notes\"\n          },\n          \"data\": {\n            \"type\": \"string\",\n            \"format\": \"byte\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-attachment-request-schema.json
tags: []
title: AttachmentRequest
---
