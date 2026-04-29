---
description: AudienceInsightsResponse from LinkedIn API
layout: schema
name: AudienceInsightsResponse
properties_list:
- description: ''
  name: value
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-insights-audience-insights-response-schema.json
slug: linkedin-marketing-audience-insights-audience-insights-response
source_filename: linkedin-marketing-audience-insights-audience-insights-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-audience-insights-response-schema.json\",\n  \"title\": \"AudienceInsightsResponse\",\n  \"description\": \"AudienceInsightsResponse from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"audienceInsight\": {\n          \"$ref\": \"#/components/schemas/AudienceInsight\"\n        },\n        \"totalAudienceCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Total count of the target audience\",\n          \"example\": 5500000\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-audience-insights-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AudienceInsightsResponse
---
