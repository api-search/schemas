---
description: Event
layout: schema
name: event
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: actor
  type: object
- description: ''
  name: repo
  type: object
- description: ''
  name: org
  type: object
- description: ''
  name: payload
  type: object
- description: ''
  name: public
  type: boolean
- description: ''
  name: created_at
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-networks-event-schema.json
slug: github-networks-event
source_filename: github-networks-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-networks-event-schema.json\",\n  \"title\": \"event\",\n  \"description\": \"Event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"12345678\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"User\"\n    },\n    \"actor\": {\n      \"$ref\": \"#/components/schemas/actor\"\n    },\n    \"repo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"url\"\n      ]\n    },\n    \"org\": {\n\
  \      \"$ref\": \"#/components/schemas/actor\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"action\": {\n          \"type\": \"string\"\n        },\n        \"issue\": {\n          \"$ref\": \"#/components/schemas/issue\"\n        },\n        \"comment\": {\n          \"$ref\": \"#/components/schemas/issue-comment\"\n        },\n        \"pages\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"page_name\": {\n                \"type\": \"string\"\n              },\n              \"title\": {\n                \"type\": \"string\"\n              },\n              \"summary\": {\n                \"type\": \"string\",\n                \"nullable\": true\n              },\n              \"action\": {\n                \"type\": \"string\"\n              },\n              \"sha\": {\n                \"type\": \"string\"\n              },\n             \
  \ \"html_url\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"public\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"example\": \"2026-04-17T12:00:00Z\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"actor\",\n    \"repo\",\n    \"payload\",\n    \"public\",\n    \"created_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-networks-event-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: event
---
