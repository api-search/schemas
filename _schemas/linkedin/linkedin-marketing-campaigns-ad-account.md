---
description: AdAccount from LinkedIn API
layout: schema
name: AdAccount
properties_list:
- description: Unique identifier
  name: id
  type: integer
- description: Display name
  name: name
  type: string
- description: Account currency
  name: currency
  type: string
- description: Account type
  name: type
  type: string
- description: Account status
  name: status
  type: string
- description: Organization URN
  name: reference
  type: string
- description: Whether this is a test account
  name: test
  type: boolean
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
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-ad-account-schema.json
slug: linkedin-marketing-campaigns-ad-account
source_filename: linkedin-marketing-campaigns-ad-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-ad-account-schema.json\",\n  \"title\": \"AdAccount\",\n  \"description\": \"AdAccount from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unique identifier\",\n      \"example\": 123456\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name\",\n      \"example\": \"XYZ Company\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Account currency\",\n      \"example\": \"USD\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"BUSINESS\",\n        \"ENTERPRISE\"\n      ],\n      \"description\": \"Account type\",\n      \"example\": \"BUSINESS\"\n    },\n    \"status\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"CANCELLED\",\n        \"DRAFT\",\n        \"PENDING_DELETION\",\n        \"REMOVED\"\n      ],\n      \"description\": \"Account status\",\n      \"example\": \"ACTIVE\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Organization URN\",\n      \"example\": \"urn:li:organization:12345678\"\n    },\n    \"test\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a test account\",\n      \"example\": true\n    },\n    \"notifiedOnCampaignOptimization\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"notifiedOnCreativeApproval\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"notifiedOnCreativeRejection\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"notifiedOnEndOfCampaign\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-ad-account-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AdAccount
---
