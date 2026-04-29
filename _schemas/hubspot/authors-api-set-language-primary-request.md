---
description: Request to set a new primary language for a multi-language group
layout: schema
name: SetLanguagePrimaryRequest
properties_list:
- description: ID of the author to set as primary
  name: id
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/authors-api-set-language-primary-request-schema.json
slug: authors-api-set-language-primary-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-set-language-primary-request-schema.json\",\n  \"title\": \"SetLanguagePrimaryRequest\",\n  \"description\": \"Request to set a new primary language for a multi-language group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the author to set as primary\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-set-language-primary-request-schema.json
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
