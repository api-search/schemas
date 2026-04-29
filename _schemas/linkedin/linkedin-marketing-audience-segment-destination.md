---
description: SegmentDestination from LinkedIn API
layout: schema
name: SegmentDestination
properties_list:
- description: Destination platform
  name: destination
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-segment-destination-schema.json
slug: linkedin-marketing-audience-segment-destination
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-segment-destination-schema.json\",\n  \"title\": \"SegmentDestination\",\n  \"description\": \"SegmentDestination from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destination\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LINKEDIN\"\n      ],\n      \"description\": \"Destination platform\",\n      \"example\": \"LINKEDIN\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-segment-destination-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: SegmentDestination
---
