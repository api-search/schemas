---
description: Request to create a language variation of an author
layout: schema
name: CreateLanguageVariationRequest
properties_list:
- description: ID of the source author
  name: id
  type: string
- description: Language code for the new variation
  name: language
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/authors-api-create-language-variation-request-schema.json
slug: authors-api-create-language-variation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-create-language-variation-request-schema.json\",\n  \"title\": \"CreateLanguageVariationRequest\",\n  \"description\": \"Request to create a language variation of an author\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the source author\",\n      \"example\": \"500123\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language code for the new variation\",\n      \"example\": \"en\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"language\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-create-language-variation-request-schema.json
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
title: CreateLanguageVariationRequest
---
