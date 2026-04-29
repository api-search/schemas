---
description: Request body for creating a reply to a comment
layout: schema
name: CreateReplyRequest
properties_list:
- description: Reply text (1-2048 characters)
  name: message
  type: string
provider_name: Canva
provider_slug: canva
schema_file: json-schema/canva-connect-create-reply-request-schema.json
slug: canva-connect-create-reply-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateReplyRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a reply to a comment\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Reply text (1-2048 characters)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/canva/refs/heads/main/json-schema/canva-connect-create-reply-request-schema.json
tags:
- Apps
- Automation
- Brand Management
- Collaboration
- Design
- Graphics
- Marketing
- Print
- Templates
- Visual Content
title: CreateReplyRequest
---
