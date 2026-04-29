---
description: Represents a participant in a conversation (visitor, agent, or bot).
layout: schema
name: Actor
properties_list:
- description: Unique identifier for the actor
  name: id
  type: string
- description: Actor ID reference
  name: actorId
  type: string
- description: Display name of the actor
  name: name
  type: string
- description: Email address of the actor
  name: email
  type: string
- description: Type of actor (e.g., VISITOR, AGENT, BOT)
  name: type
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-conversations-actor-schema.json
slug: hubspot-conversations-actor
source_filename: hubspot-conversations-actor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents a participant in a conversation (visitor, agent, or bot).\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the actor\",\n      \"example\": \"actor_101\"\n    },\n    \"actorId\": {\n      \"type\": \"string\",\n      \"description\": \"Actor ID reference\",\n      \"example\": \"actor_101\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the actor\",\n      \"example\": \"John Customer\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address of the actor\",\n      \"format\": \"email\",\n      \"example\": \"john@example.com\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of actor (e.g., VISITOR, AGENT, BOT)\",\n      \"example\": \"VISITOR\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"Actor\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-conversations-actor-schema.json
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
title: Actor
---
