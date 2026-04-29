---
description: AdAccountUser from LinkedIn API
layout: schema
name: AdAccountUser
properties_list:
- description: URN of the sponsored account
  name: account
  type: string
- description: URN of the person
  name: user
  type: string
- description: Role of the user in the account
  name: role
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-ad-account-user-schema.json
slug: linkedin-marketing-campaigns-ad-account-user
source_filename: linkedin-marketing-campaigns-ad-account-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-ad-account-user-schema.json\",\n  \"title\": \"AdAccountUser\",\n  \"description\": \"AdAccountUser from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the sponsored account\",\n      \"example\": \"urn:li:sponsoredAccount:123456\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the person\",\n      \"example\": \"urn:li:person:ABC123def\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACCOUNT_BILLING_ADMIN\",\n        \"ACCOUNT_MANAGER\",\n        \"CAMPAIGN_MANAGER\",\n        \"CREATIVE_MANAGER\",\n        \"VIEWER\"\n      ],\n      \"description\": \"Role of the user in the account\",\n      \"example\": \"\
  VIEWER\"\n    }\n  },\n  \"required\": [\n    \"account\",\n    \"user\",\n    \"role\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-ad-account-user-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AdAccountUser
---
