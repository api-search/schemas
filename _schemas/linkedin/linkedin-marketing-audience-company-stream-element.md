---
description: CompanyStreamElement from LinkedIn API
layout: schema
name: CompanyStreamElement
properties_list:
- description: Action to perform
  name: action
  type: string
- description: Company name to add or remove
  name: companyName
  type: string
- description: Company domain (optional)
  name: companyDomain
  type: string
- description: Company LinkedIn page URL (optional)
  name: companyPageUrl
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-company-stream-element-schema.json
slug: linkedin-marketing-audience-company-stream-element
source_filename: linkedin-marketing-audience-company-stream-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-company-stream-element-schema.json\",\n  \"title\": \"CompanyStreamElement\",\n  \"description\": \"CompanyStreamElement from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ADD\",\n        \"REMOVE\"\n      ],\n      \"description\": \"Action to perform\",\n      \"example\": \"ADD\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"Company name to add or remove\",\n      \"example\": \"LinkedIn\"\n    },\n    \"companyDomain\": {\n      \"type\": \"string\",\n      \"description\": \"Company domain (optional)\",\n      \"example\": \"linkedin.com\"\n    },\n    \"companyPageUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Company LinkedIn\
  \ page URL (optional)\",\n      \"example\": \"https://www.linkedin.com/company/linkedin\"\n    }\n  },\n  \"required\": [\n    \"action\",\n    \"companyName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-company-stream-element-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: CompanyStreamElement
---
