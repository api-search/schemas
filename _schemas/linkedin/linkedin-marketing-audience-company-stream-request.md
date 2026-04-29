---
description: CompanyStreamRequest from LinkedIn API
layout: schema
name: CompanyStreamRequest
properties_list:
- description: ''
  name: elements
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-company-stream-request-schema.json
slug: linkedin-marketing-audience-company-stream-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-company-stream-request-schema.json\",\n  \"title\": \"CompanyStreamRequest\",\n  \"description\": \"CompanyStreamRequest from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CompanyStreamElement\"\n      }\n    }\n  },\n  \"required\": [\n    \"elements\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-company-stream-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: CompanyStreamRequest
---
