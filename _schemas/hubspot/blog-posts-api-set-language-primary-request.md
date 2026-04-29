---
description: Request to set new primary language
layout: schema
name: SetLanguagePrimaryRequest
properties_list:
- description: ID of the post to set as primary
  name: id
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/blog-posts-api-set-language-primary-request-schema.json
slug: blog-posts-api-set-language-primary-request
source_filename: blog-posts-api-set-language-primary-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-set-language-primary-request-schema.json\",\n  \"title\": \"SetLanguagePrimaryRequest\",\n  \"description\": \"Request to set new primary language\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the post to set as primary\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-set-language-primary-request-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: SetLanguagePrimaryRequest
---
