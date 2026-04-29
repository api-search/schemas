---
description: Request to schedule a blog post for publication
layout: schema
name: ScheduleRequest
properties_list:
- description: ID of the blog post to schedule
  name: id
  type: string
- description: ISO 8601 date and time to publish
  name: publishDate
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/blog-posts-api-schedule-request-schema.json
slug: blog-posts-api-schedule-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-schedule-request-schema.json\",\n  \"title\": \"ScheduleRequest\",\n  \"description\": \"Request to schedule a blog post for publication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the blog post to schedule\",\n      \"example\": \"500123\"\n    },\n    \"publishDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 date and time to publish\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"publishDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-schedule-request-schema.json
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
title: ScheduleRequest
---
