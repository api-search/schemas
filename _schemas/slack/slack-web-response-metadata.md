---
description: Metadata for paginated responses containing cursor information.
layout: schema
name: ResponseMetadata
properties_list:
- description: An opaque cursor to use in the next request to get the next page of results. Empty string indicates no more results.
  name: next_cursor
  type: string
provider_name: Slack
provider_slug: slack
schema_file: json-schema/slack-web-response-metadata-schema.json
slug: slack-web-response-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseMetadata\",\n  \"type\": \"object\",\n  \"description\": \"Metadata for paginated responses containing cursor information.\",\n  \"properties\": {\n    \"next_cursor\": {\n      \"type\": \"string\",\n      \"description\": \"An opaque cursor to use in the next request to get the next page of results. Empty string indicates no more results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/slack/refs/heads/main/json-schema/slack-web-response-metadata-schema.json
tags:
- Bots
- Chat
- Collaboration
- Messaging
- Productivity
- T1
- Team Communication
title: ResponseMetadata
---
