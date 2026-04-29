---
description: DmpSegment from LinkedIn API
layout: schema
name: DmpSegment
properties_list:
- description: Unique identifier for the DMP segment
  name: id
  type: integer
- description: Display name of the segment
  name: name
  type: string
- description: URN of the sponsore account
  name: account
  type: string
- description: Access policy for the segment
  name: accessPolicy
  type: string
- description: Type of DMP segment
  name: type
  type: string
- description: Source platform for the segment data
  name: sourcePlatform
  type: string
- description: Current status of the segment
  name: status
  type: string
- description: Number of matched records
  name: matchedCount
  type: integer
- description: Total number of input records
  name: inputCount
  type: integer
- description: Size of the audience
  name: audienceSize
  type: integer
- description: ''
  name: destinations
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-dmp-segment-schema.json
slug: linkedin-marketing-audience-dmp-segment
source_filename: linkedin-marketing-audience-dmp-segment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-dmp-segment-schema.json\",\n  \"title\": \"DmpSegment\",\n  \"description\": \"DmpSegment from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unique identifier for the DMP segment\",\n      \"example\": 987654321\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the segment\",\n      \"example\": \"DMP segment for CSV uploads\"\n    },\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the sponsore account\",\n      \"example\": \"urn:li:sponsoredAccount:123456\"\n    },\n    \"accessPolicy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PRIVATE\",\n        \"PUBLIC\"\n      ],\n\
  \      \"description\": \"Access policy for the segment\",\n      \"example\": \"PRIVATE\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"COMPANY_LIST_UPLOAD\",\n        \"USER_LIST_UPLOAD\",\n        \"COMPANY_STREAMING\",\n        \"USER_STREAMING\"\n      ],\n      \"description\": \"Type of DMP segment\",\n      \"example\": \"COMPANY_LIST_UPLOAD\"\n    },\n    \"sourcePlatform\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LIST_UPLOAD\",\n        \"STREAMING\"\n      ],\n      \"description\": \"Source platform for the segment data\",\n      \"example\": \"LIST_UPLOAD\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PROCESSING\",\n        \"READY\",\n        \"EXPIRED\",\n        \"FAILED\"\n      ],\n      \"description\": \"Current status of the segment\",\n      \"example\": \"READY\"\n    },\n    \"matchedCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of matched\
  \ records\",\n      \"example\": 5000\n    },\n    \"inputCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of input records\",\n      \"example\": 6000\n    },\n    \"audienceSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the audience\",\n      \"example\": 4500\n    },\n    \"destinations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SegmentDestination\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"account\",\n    \"type\",\n    \"sourcePlatform\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-dmp-segment-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: DmpSegment
---
