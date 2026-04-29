---
description: UserStreamElement from LinkedIn API
layout: schema
name: UserStreamElement
properties_list:
- description: Action to perform
  name: action
  type: string
- description: ''
  name: userIds
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-user-stream-element-schema.json
slug: linkedin-marketing-audience-user-stream-element
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-user-stream-element-schema.json\",\n  \"title\": \"UserStreamElement\",\n  \"description\": \"UserStreamElement from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ADD\",\n        \"REMOVE\"\n      ],\n      \"description\": \"Action to perform\",\n      \"example\": \"ADD\"\n    },\n    \"userIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserId\"\n      }\n    }\n  },\n  \"required\": [\n    \"action\",\n    \"userIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-user-stream-element-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: UserStreamElement
---
