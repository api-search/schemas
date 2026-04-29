---
description: A paginated list of events.
layout: schema
name: EventPage
properties_list:
- description: The list of events.
  name: data
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-event-page-schema.json
slug: atlassian-admin-event-page
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventPage\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of events.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of events.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-event-page-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: EventPage
---
