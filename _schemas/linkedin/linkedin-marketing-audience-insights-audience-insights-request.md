---
description: AudienceInsightsRequest from LinkedIn API
layout: schema
name: AudienceInsightsRequest
properties_list:
- description: ''
  name: request
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-insights-audience-insights-request-schema.json
slug: linkedin-marketing-audience-insights-audience-insights-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-audience-insights-request-schema.json\",\n  \"title\": \"AudienceInsightsRequest\",\n  \"description\": \"AudienceInsightsRequest from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"requestMetaData\": {\n          \"$ref\": \"#/components/schemas/RequestMetaData\"\n        },\n        \"targetingCriteria\": {\n          \"$ref\": \"#/components/schemas/TargetingCriteria\"\n        },\n        \"groupBy\": {\n          \"type\": \"string\",\n          \"description\": \"Facet URN to group insights by\",\n          \"example\": \"urn:li:adTargetingFacet:interests\"\n        }\n      },\n      \"required\": [\n        \"targetingCriteria\",\n        \"groupBy\"\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-audience-insights-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AudienceInsightsRequest
---
