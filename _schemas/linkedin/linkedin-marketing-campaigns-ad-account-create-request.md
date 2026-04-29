---
description: AdAccountCreateRequest from LinkedIn API
layout: schema
name: AdAccountCreateRequest
properties_list:
- description: ''
  name: currency
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: notifiedOnCampaignOptimization
  type: boolean
- description: ''
  name: notifiedOnCreativeApproval
  type: boolean
- description: ''
  name: notifiedOnCreativeRejection
  type: boolean
- description: ''
  name: notifiedOnEndOfCampaign
  type: boolean
- description: ''
  name: reference
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: test
  type: boolean
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-ad-account-create-request-schema.json
slug: linkedin-marketing-campaigns-ad-account-create-request
source_filename: linkedin-marketing-campaigns-ad-account-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-ad-account-create-request-schema.json\",\n  \"title\": \"AdAccountCreateRequest\",\n  \"description\": \"AdAccountCreateRequest from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"type\": \"string\",\n      \"example\": \"USD\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"XYZ Company\"\n    },\n    \"notifiedOnCampaignOptimization\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"notifiedOnCreativeApproval\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"notifiedOnCreativeRejection\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"notifiedOnEndOfCampaign\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"reference\"\
  : {\n      \"type\": \"string\",\n      \"example\": \"urn:li:organization:12345678\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"BUSINESS\",\n        \"ENTERPRISE\"\n      ],\n      \"example\": \"BUSINESS\"\n    },\n    \"test\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"currency\",\n    \"name\",\n    \"reference\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-ad-account-create-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AdAccountCreateRequest
---
