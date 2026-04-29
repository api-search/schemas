---
description: Request to attach to language group
layout: schema
name: AttachToLanguageGroupRequest
properties_list:
- description: ID of the post to attach
  name: id
  type: string
- description: Language code for the post
  name: language
  type: string
- description: ID of the primary language post
  name: primaryId
  type: string
- description: Language code of the primary post
  name: primaryLanguage
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/blog-posts-api-attach-to-language-group-request-schema.json
slug: blog-posts-api-attach-to-language-group-request
source_filename: blog-posts-api-attach-to-language-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-attach-to-language-group-request-schema.json\",\n  \"title\": \"AttachToLanguageGroupRequest\",\n  \"description\": \"Request to attach to language group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the post to attach\",\n      \"example\": \"500123\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language code for the post\",\n      \"example\": \"en\"\n    },\n    \"primaryId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the primary language post\",\n      \"example\": \"500123\"\n    },\n    \"primaryLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"Language code of the primary post\",\n      \"example\": \"en\"\n    }\n  },\n  \"required\"\
  : [\n    \"id\",\n    \"language\",\n    \"primaryId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-attach-to-language-group-request-schema.json
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
