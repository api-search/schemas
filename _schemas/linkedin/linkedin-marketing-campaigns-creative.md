---
description: Creative from LinkedIn API
layout: schema
name: Creative
properties_list:
- description: Creative URN
  name: id
  type: string
- description: Parent campaign URN
  name: campaign
  type: string
- description: Reference URN (e.g., UGC post)
  name: reference
  type: string
- description: Creative status
  name: status
  type: string
- description: Creative type
  name: type
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-creative-schema.json
slug: linkedin-marketing-campaigns-creative
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-creative-schema.json\",\n  \"title\": \"Creative\",\n  \"description\": \"Creative from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Creative URN\",\n      \"example\": \"urn:li:sponsoredCreative:777888999\"\n    },\n    \"campaign\": {\n      \"type\": \"string\",\n      \"description\": \"Parent campaign URN\",\n      \"example\": \"urn:li:sponsoredCampaign:444555666\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Reference URN (e.g., UGC post)\",\n      \"example\": \"urn:li:ugcPost:123456789\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"PAUSED\",\n        \"DRAFT\",\n        \"ARCHIVED\",\n\
  \        \"CANCELLED\",\n        \"PENDING_DELETION\",\n        \"REMOVED\"\n      ],\n      \"description\": \"Creative status\",\n      \"example\": \"ACTIVE\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SPONSORED_STATUS_UPDATE\",\n        \"SPONSORED_VIDEO\",\n        \"CAROUSEL\",\n        \"TEXT_AD\",\n        \"MESSAGE_AD\"\n      ],\n      \"description\": \"Creative type\",\n      \"example\": \"SPONSORED_VIDEO\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-creative-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: Creative
---
