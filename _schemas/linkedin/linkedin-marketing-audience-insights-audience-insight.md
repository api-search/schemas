---
description: AudienceInsight from LinkedIn API
layout: schema
name: AudienceInsight
properties_list:
- description: ''
  name: segmentations
  type: array
- description: Facet URN the insights are grouped by
  name: groupedBy
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-insights-audience-insight-schema.json
slug: linkedin-marketing-audience-insights-audience-insight
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-audience-insight-schema.json\",\n  \"title\": \"AudienceInsight\",\n  \"description\": \"AudienceInsight from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"segmentations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InsightSegmentation\"\n      }\n    },\n    \"groupedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Facet URN the insights are grouped by\",\n      \"example\": \"urn:li:adTargetingFacet:interests\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-audience-insight-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AudienceInsight
---
