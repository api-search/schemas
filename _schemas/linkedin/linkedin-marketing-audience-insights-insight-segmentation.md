---
description: InsightSegmentation from LinkedIn API
layout: schema
name: InsightSegmentation
properties_list:
- description: Number of members matching this segment
  name: entityCount
  type: integer
- description: Percentage of audience matching this segment
  name: entityPercentage
  type: integer
- description: URN of the segment value
  name: value
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-insights-insight-segmentation-schema.json
slug: linkedin-marketing-audience-insights-insight-segmentation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-insight-segmentation-schema.json\",\n  \"title\": \"InsightSegmentation\",\n  \"description\": \"InsightSegmentation from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of members matching this segment\",\n      \"example\": 4900000\n    },\n    \"entityPercentage\": {\n      \"type\": \"integer\",\n      \"description\": \"Percentage of audience matching this segment\",\n      \"example\": 89\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the segment value\",\n      \"example\": \"urn:li:interest:71363\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-insight-segmentation-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: InsightSegmentation
---
