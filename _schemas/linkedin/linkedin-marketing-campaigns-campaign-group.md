---
description: CampaignGroup from LinkedIn API
layout: schema
name: CampaignGroup
properties_list:
- description: Unique identifier
  name: id
  type: integer
- description: Display name
  name: name
  type: string
- description: Parent account URN
  name: account
  type: string
- description: Campaign group status
  name: status
  type: string
- description: ''
  name: totalBudget
  type: object
- description: ''
  name: runSchedule
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-campaign-group-schema.json
slug: linkedin-marketing-campaigns-campaign-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-campaign-group-schema.json\",\n  \"title\": \"CampaignGroup\",\n  \"description\": \"CampaignGroup from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unique identifier\",\n      \"example\": 111222333\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name\",\n      \"example\": \"Q1 2024 Campaign Group\"\n    },\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"Parent account URN\",\n      \"example\": \"urn:li:sponsoredAccount:123456\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"ARCHIVED\",\n        \"CANCELLED\",\n        \"DRAFT\",\n     \
  \   \"PAUSED\",\n        \"PENDING_DELETION\",\n        \"REMOVED\"\n      ],\n      \"description\": \"Campaign group status\",\n      \"example\": \"ACTIVE\"\n    },\n    \"totalBudget\": {\n      \"$ref\": \"#/components/schemas/Budget\"\n    },\n    \"runSchedule\": {\n      \"$ref\": \"#/components/schemas/RunSchedule\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-campaign-group-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: CampaignGroup
---
