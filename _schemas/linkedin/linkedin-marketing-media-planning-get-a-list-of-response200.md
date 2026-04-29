---
description: GetAListOfResponse200 from LinkedIn API
layout: schema
name: GetAListOfResponse200
properties_list:
- description: ''
  name: paging
  type: object
- description: ''
  name: elements
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-media-planning-get-a-list-of-response200-schema.json
slug: linkedin-marketing-media-planning-get-a-list-of-response200
source_filename: linkedin-marketing-media-planning-get-a-list-of-response200-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-media-planning-get-a-list-of-response200-schema.json\",\n  \"title\": \"GetAListOfResponse200\",\n  \"description\": \"GetAListOfResponse200 from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paging\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"integer\"\n        },\n        \"count\": {\n          \"type\": \"integer\"\n        },\n        \"links\": {\n          \"type\": \"array\",\n          \"items\": {}\n        }\n      }\n    },\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"entityTypes\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n         \
  \ },\n          \"facetName\": {\n            \"type\": \"string\"\n          },\n          \"availableEntityFinders\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-media-planning-get-a-list-of-response200-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: GetAListOfResponse200
---
