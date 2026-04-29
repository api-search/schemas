---
description: TargetingCriteria from LinkedIn API
layout: schema
name: TargetingCriteria
properties_list:
- description: ''
  name: include
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-insights-targeting-criteria-schema.json
slug: linkedin-marketing-audience-insights-targeting-criteria
source_filename: linkedin-marketing-audience-insights-targeting-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-targeting-criteria-schema.json\",\n  \"title\": \"TargetingCriteria\",\n  \"description\": \"TargetingCriteria from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"include\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"and\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"or\": {\n                \"type\": \"object\",\n                \"additionalProperties\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-targeting-criteria-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: TargetingCriteria
---
