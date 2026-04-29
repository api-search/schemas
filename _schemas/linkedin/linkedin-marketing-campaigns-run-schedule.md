---
description: RunSchedule from LinkedIn API
layout: schema
name: RunSchedule
properties_list:
- description: Start timestamp in milliseconds
  name: start
  type: integer
- description: End timestamp in milliseconds
  name: end
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-run-schedule-schema.json
slug: linkedin-marketing-campaigns-run-schedule
source_filename: linkedin-marketing-campaigns-run-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-run-schedule-schema.json\",\n  \"title\": \"RunSchedule\",\n  \"description\": \"RunSchedule from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Start timestamp in milliseconds\",\n      \"example\": 1647927789001\n    },\n    \"end\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"End timestamp in milliseconds\",\n      \"example\": 1648186989000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-run-schedule-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: RunSchedule
---
