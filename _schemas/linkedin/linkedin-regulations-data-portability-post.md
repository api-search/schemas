---
description: Post from LinkedIn API
layout: schema
name: Post
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: author
  type: string
- description: ''
  name: commentary
  type: string
- description: ''
  name: visibility
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: created
  type: object
- description: ''
  name: lastModified
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-regulations-data-portability-post-schema.json
slug: linkedin-regulations-data-portability-post
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-post-schema.json\",\n  \"title\": \"Post\",\n  \"description\": \"Post from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"urn:li:share:7012345678901234567\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"example\": \"urn:li:organization:10002687\"\n    },\n    \"commentary\": {\n      \"type\": \"string\",\n      \"example\": \"Exciting news from our team!\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PUBLIC\",\n        \"CONNECTIONS\"\n      ],\n      \"example\": \"PUBLIC\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PUBLISHED\",\n        \"DRAFT\"\n      ],\n      \"example\"\
  : \"PUBLISHED\"\n    },\n    \"created\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    },\n    \"lastModified\": {\n      \"$ref\": \"#/components/schemas/Timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-post-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: Post
---
