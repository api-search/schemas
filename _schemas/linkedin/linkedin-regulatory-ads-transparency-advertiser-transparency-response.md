---
description: AdvertiserTransparencyResponse from LinkedIn API
layout: schema
name: AdvertiserTransparencyResponse
properties_list:
- description: The URN of the sponsored account
  name: sponsoredAccountUrn
  type: string
- description: The month of the transparency data
  name: month
  type: integer
- description: Total advertising spend for the month
  name: totalSpend
  type: number
- description: Total impressions delivered
  name: impressions
  type: integer
- description: Currency code for spend amounts
  name: currency
  type: string
- description: Name of the advertiser
  name: advertiserName
  type: string
- description: Country of the advertiser
  name: country
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-regulatory-ads-transparency-advertiser-transparency-response-schema.json
slug: linkedin-regulatory-ads-transparency-advertiser-transparency-response
source_filename: linkedin-regulatory-ads-transparency-advertiser-transparency-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulatory-ads-transparency-advertiser-transparency-response-schema.json\",\n  \"title\": \"AdvertiserTransparencyResponse\",\n  \"description\": \"AdvertiserTransparencyResponse from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sponsoredAccountUrn\": {\n      \"type\": \"string\",\n      \"description\": \"The URN of the sponsored account\",\n      \"example\": \"urn:li:sponsoredAccount:123456789\"\n    },\n    \"month\": {\n      \"type\": \"integer\",\n      \"description\": \"The month of the transparency data\",\n      \"example\": 202312\n    },\n    \"totalSpend\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total advertising spend for the month\",\n      \"example\": 15000.5\n    },\n    \"impressions\": {\n      \"type\": \"\
  integer\",\n      \"description\": \"Total impressions delivered\",\n      \"example\": 500000\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code for spend amounts\",\n      \"example\": \"USD\"\n    },\n    \"advertiserName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the advertiser\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country of the advertiser\",\n      \"example\": \"United States\"\n    }\n  },\n  \"required\": [\n    \"sponsoredAccountUrn\",\n    \"month\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulatory-ads-transparency-advertiser-transparency-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AdvertiserTransparencyResponse
---
