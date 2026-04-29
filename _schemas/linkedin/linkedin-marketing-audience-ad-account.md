---
description: AdAccount from LinkedIn API
layout: schema
name: AdAccount
properties_list:
- description: Unique identifier for the ad account
  name: id
  type: integer
- description: Display name of the ad account
  name: name
  type: string
- description: Reference URN (organization) for the ad account
  name: reference
  type: string
- description: Whether this is a test ad account
  name: test
  type: boolean
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-ad-account-schema.json
slug: linkedin-marketing-audience-ad-account
source_filename: linkedin-marketing-audience-ad-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-ad-account-schema.json\",\n  \"title\": \"AdAccount\",\n  \"description\": \"AdAccount from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unique identifier for the ad account\",\n      \"example\": 123456\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the ad account\",\n      \"example\": \"Test ad account\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Reference URN (organization) for the ad account\",\n      \"example\": \"urn:li:organization:11223344\"\n    },\n    \"test\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a test ad account\",\n      \"\
  example\": false\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"test\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-ad-account-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AdAccount
---
