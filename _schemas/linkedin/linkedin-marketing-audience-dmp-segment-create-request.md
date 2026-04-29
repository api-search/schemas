---
description: DmpSegmentCreateRequest from LinkedIn API
layout: schema
name: DmpSegmentCreateRequest
properties_list:
- description: Access policy for the segment
  name: accessPolicy
  type: string
- description: URN of the sponsored account
  name: account
  type: string
- description: ''
  name: destinations
  type: array
- description: Display name for the segment
  name: name
  type: string
- description: Source platform
  name: sourcePlatform
  type: string
- description: Type of segment
  name: type
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-dmp-segment-create-request-schema.json
slug: linkedin-marketing-audience-dmp-segment-create-request
source_filename: linkedin-marketing-audience-dmp-segment-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-dmp-segment-create-request-schema.json\",\n  \"title\": \"DmpSegmentCreateRequest\",\n  \"description\": \"DmpSegmentCreateRequest from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessPolicy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PRIVATE\",\n        \"PUBLIC\"\n      ],\n      \"description\": \"Access policy for the segment\",\n      \"example\": \"PRIVATE\"\n    },\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the sponsored account\",\n      \"example\": \"urn:li:sponsoredAccount:123456\"\n    },\n    \"destinations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SegmentDestination\"\n      }\n    },\n    \"name\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Display name for the segment\",\n      \"example\": \"DMP segment for CSV uploads\"\n    },\n    \"sourcePlatform\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LIST_UPLOAD\",\n        \"STREAMING\"\n      ],\n      \"description\": \"Source platform\",\n      \"example\": \"LIST_UPLOAD\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"COMPANY_LIST_UPLOAD\",\n        \"USER_LIST_UPLOAD\",\n        \"COMPANY_STREAMING\",\n        \"USER_STREAMING\"\n      ],\n      \"description\": \"Type of segment\",\n      \"example\": \"COMPANY_LIST_UPLOAD\"\n    }\n  },\n  \"required\": [\n    \"accessPolicy\",\n    \"account\",\n    \"destinations\",\n    \"name\",\n    \"sourcePlatform\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-dmp-segment-create-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: DmpSegmentCreateRequest
---
