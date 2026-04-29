---
description: Request to restore a previous version
layout: schema
name: RestorePreviousVersionRequest
properties_list:
- description: ID of the blog post
  name: id
  type: string
- description: ID of the revision to restore
  name: revisionId
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/blog-posts-api-restore-previous-version-request-schema.json
slug: blog-posts-api-restore-previous-version-request
source_filename: blog-posts-api-restore-previous-version-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-restore-previous-version-request-schema.json\",\n  \"title\": \"RestorePreviousVersionRequest\",\n  \"description\": \"Request to restore a previous version\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the blog post\",\n      \"example\": \"500123\"\n    },\n    \"revisionId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the revision to restore\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"revisionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-restore-previous-version-request-schema.json
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
title: RestorePreviousVersionRequest
---
