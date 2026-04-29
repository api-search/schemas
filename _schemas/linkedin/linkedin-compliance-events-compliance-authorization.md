---
description: ComplianceAuthorization from LinkedIn API
layout: schema
name: ComplianceAuthorization
properties_list:
- description: URN of the developer application
  name: developerApplication
  type: string
- description: URN of the regulated member
  name: member
  type: string
- description: Authorization status of the member
  name: status
  type: string
- description: Timestamp when authorization was created
  name: createdAt
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-compliance-events-compliance-authorization-schema.json
slug: linkedin-compliance-events-compliance-authorization
source_filename: linkedin-compliance-events-compliance-authorization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-compliance-events-compliance-authorization-schema.json\",\n  \"title\": \"ComplianceAuthorization\",\n  \"description\": \"ComplianceAuthorization from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"developerApplication\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the developer application\",\n      \"example\": \"urn:li:developerApplication:12345678\"\n    },\n    \"member\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the regulated member\",\n      \"example\": \"urn:li:person:ABC123def\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AUTHORIZED\",\n        \"UNAUTHORIZED\"\n      ],\n      \"description\": \"Authorization status of the member\",\n      \"example\": \"AUTHORIZED\"\n    },\n    \"\
  createdAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Timestamp when authorization was created\",\n      \"example\": 1640000000000\n    }\n  },\n  \"required\": [\n    \"developerApplication\",\n    \"member\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-compliance-events-compliance-authorization-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ComplianceAuthorization
---
