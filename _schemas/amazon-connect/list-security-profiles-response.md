---
description: ListSecurityProfilesResponse schema from Amazon Connect Service API
layout: schema
name: ListSecurityProfilesResponse
properties_list:
- description: ''
  name: SecurityProfileSummaryList
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/list-security-profiles-response-schema.json
slug: list-security-profiles-response
source_filename: list-security-profiles-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-security-profiles-response-schema.json\",\n  \"title\": \"ListSecurityProfilesResponse\",\n  \"description\": \"ListSecurityProfilesResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SecurityProfileSummaryList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SecurityProfileSummary\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/list-security-profiles-response-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: ListSecurityProfilesResponse
---
