---
description: Payload for creating or updating a segment
layout: schema
name: SegmentCreate
properties_list:
- description: Display name of the segment
  name: name
  type: string
- description: Description of the segment's purpose
  name: description
  type: string
- description: Report suite ID this segment is based on
  name: rsid
  type: string
- description: The segment rule definition in Analytics query format
  name: definition
  type: object
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-segment-create-schema.json
slug: adobe-analytics-segment-create
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Payload for creating or updating a segment\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the segment\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the segment's purpose\",\n      \"example\": \"A sample description.\"\n    },\n    \"rsid\": {\n      \"type\": \"string\",\n      \"description\": \"Report suite ID this segment is based on\",\n      \"example\": \"500123\"\n    },\n    \"definition\": {\n      \"type\": \"object\",\n      \"description\": \"The segment rule definition in Analytics query format\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"rsid\",\n    \"definition\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SegmentCreate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-segment-create-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: SegmentCreate
---
