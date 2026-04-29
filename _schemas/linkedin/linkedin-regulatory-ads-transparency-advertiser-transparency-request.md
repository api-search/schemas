---
description: AdvertiserTransparencyRequest from LinkedIn API
layout: schema
name: AdvertiserTransparencyRequest
properties_list:
- description: The unique identifier for the sponsored account
  name: sponsoredAccountId
  type: string
- description: The month for transparency data in YYYYMM format
  name: month
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-regulatory-ads-transparency-advertiser-transparency-request-schema.json
slug: linkedin-regulatory-ads-transparency-advertiser-transparency-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulatory-ads-transparency-advertiser-transparency-request-schema.json\",\n  \"title\": \"AdvertiserTransparencyRequest\",\n  \"description\": \"AdvertiserTransparencyRequest from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sponsoredAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the sponsored account\",\n      \"example\": \"123456789\"\n    },\n    \"month\": {\n      \"type\": \"integer\",\n      \"description\": \"The month for transparency data in YYYYMM format\",\n      \"example\": 202312\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulatory-ads-transparency-advertiser-transparency-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AdvertiserTransparencyRequest
---
