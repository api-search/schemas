---
description: CreativeCreateRequest from LinkedIn API
layout: schema
name: CreativeCreateRequest
properties_list:
- description: ''
  name: campaign
  type: string
- description: ''
  name: reference
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: variables
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-creative-create-request-schema.json
slug: linkedin-marketing-campaigns-creative-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-creative-create-request-schema.json\",\n  \"title\": \"CreativeCreateRequest\",\n  \"description\": \"CreativeCreateRequest from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaign\": {\n      \"type\": \"string\",\n      \"example\": \"urn:li:sponsoredCampaign:444555666\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"example\": \"urn:li:ugcPost:123456789\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"ACTIVE\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"SPONSORED_VIDEO\"\n    },\n    \"variables\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"object\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"campaign\"\
  ,\n    \"reference\",\n    \"status\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-creative-create-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: CreativeCreateRequest
---
