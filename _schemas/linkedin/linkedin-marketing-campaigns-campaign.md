---
description: Campaign from LinkedIn API
layout: schema
name: Campaign
properties_list:
- description: Unique identifier
  name: id
  type: integer
- description: Campaign name
  name: name
  type: string
- description: Parent account URN
  name: account
  type: string
- description: Parent campaign group URN
  name: campaignGroup
  type: string
- description: Campaign status
  name: status
  type: string
- description: Campaign type
  name: type
  type: string
- description: Campaign objective
  name: objectiveType
  type: string
- description: ''
  name: runSchedule
  type: object
- description: ''
  name: dailyBudget
  type: object
- description: ''
  name: totalBudget
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-campaign-schema.json
slug: linkedin-marketing-campaigns-campaign
source_filename: linkedin-marketing-campaigns-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-campaign-schema.json\",\n  \"title\": \"Campaign\",\n  \"description\": \"Campaign from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unique identifier\",\n      \"example\": 444555666\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign name\",\n      \"example\": \"Spring Promotion Campaign\"\n    },\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"Parent account URN\",\n      \"example\": \"urn:li:sponsoredAccount:123456\"\n    },\n    \"campaignGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Parent campaign group URN\",\n      \"example\": \"urn:li:sponsoredCampaignGroup:111222333\"\n\
  \    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"ARCHIVED\",\n        \"CANCELLED\",\n        \"DRAFT\",\n        \"PAUSED\",\n        \"PENDING_DELETION\",\n        \"REMOVED\"\n      ],\n      \"description\": \"Campaign status\",\n      \"example\": \"ACTIVE\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SPONSORED_UPDATES\",\n        \"SPONSORED_INMAILS\",\n        \"TEXT_AD\"\n      ],\n      \"description\": \"Campaign type\",\n      \"example\": \"SPONSORED_UPDATES\"\n    },\n    \"objectiveType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"BRAND_AWARENESS\",\n        \"ENGAGEMENT\",\n        \"JOB_APPLICANTS\",\n        \"LEAD_GENERATION\",\n        \"VIDEO_VIEWS\",\n        \"WEBSITE_CONVERSIONS\",\n        \"WEBSITE_VISITS\"\n      ],\n      \"description\": \"Campaign objective\",\n      \"example\": \"WEBSITE_VISITS\"\n    },\n    \"runSchedule\": {\n      \"$ref\"\
  : \"#/components/schemas/RunSchedule\"\n    },\n    \"dailyBudget\": {\n      \"$ref\": \"#/components/schemas/Budget\"\n    },\n    \"totalBudget\": {\n      \"$ref\": \"#/components/schemas/Budget\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-campaign-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: Campaign
---
