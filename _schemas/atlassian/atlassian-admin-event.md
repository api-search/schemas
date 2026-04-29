---
description: Represents an audit event that occurred within the organization, capturing actions such as user changes, policy updates, and access modifications.
layout: schema
name: Event
properties_list:
- description: The unique identifier of the event.
  name: id
  type: string
- description: The resource type.
  name: type
  type: string
- description: The event attributes.
  name: attributes
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-event-schema.json
slug: atlassian-admin-event
source_filename: atlassian-admin-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Event\",\n  \"type\": \"object\",\n  \"description\": \"Represents an audit event that occurred within the organization, capturing actions such as user changes, policy updates, and access modifications.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the event.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"The event attributes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-event-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: Event
---
