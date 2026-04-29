---
description: AudienceCount from LinkedIn API
layout: schema
name: AudienceCount
properties_list:
- description: Total audience count
  name: total
  type: integer
- description: Active member count
  name: activeCount
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-audience-count-schema.json
slug: linkedin-marketing-campaigns-audience-count
source_filename: linkedin-marketing-campaigns-audience-count-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-audience-count-schema.json\",\n  \"title\": \"AudienceCount\",\n  \"description\": \"AudienceCount from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total audience count\",\n      \"example\": 1500000\n    },\n    \"activeCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Active member count\",\n      \"example\": 1200000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-audience-count-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AudienceCount
---
