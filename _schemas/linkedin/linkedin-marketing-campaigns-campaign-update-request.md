---
description: CampaignUpdateRequest from LinkedIn API
layout: schema
name: CampaignUpdateRequest
properties_list:
- description: ''
  name: patch
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-campaign-update-request-schema.json
slug: linkedin-marketing-campaigns-campaign-update-request
source_filename: linkedin-marketing-campaigns-campaign-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-campaign-update-request-schema.json\",\n  \"title\": \"CampaignUpdateRequest\",\n  \"description\": \"CampaignUpdateRequest from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"patch\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"$set\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"status\": {\n              \"type\": \"string\",\n              \"example\": \"ARCHIVED\"\n            },\n            \"runSchedule\": {\n              \"$ref\": \"#/components/schemas/RunSchedule\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-campaign-update-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: CampaignUpdateRequest
---
