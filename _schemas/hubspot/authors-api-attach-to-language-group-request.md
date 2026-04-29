---
description: Request to attach an author to a multi-language group
layout: schema
name: AttachToLanguageGroupRequest
properties_list:
- description: ID of the author to attach
  name: id
  type: string
- description: Language code for the author (e.g., es, fr, de)
  name: language
  type: string
- description: ID of the primary language author
  name: primaryId
  type: string
- description: Language code of the primary author
  name: primaryLanguage
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/authors-api-attach-to-language-group-request-schema.json
slug: authors-api-attach-to-language-group-request
source_filename: authors-api-attach-to-language-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-attach-to-language-group-request-schema.json\",\n  \"title\": \"AttachToLanguageGroupRequest\",\n  \"description\": \"Request to attach an author to a multi-language group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the author to attach\",\n      \"example\": \"500123\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language code for the author (e.g., es, fr, de)\",\n      \"example\": \"en\"\n    },\n    \"primaryId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the primary language author\",\n      \"example\": \"500123\"\n    },\n    \"primaryLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"Language code of the primary author\",\n      \"example\"\
  : \"en\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"language\",\n    \"primaryId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-attach-to-language-group-request-schema.json
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
title: AttachToLanguageGroupRequest
---
