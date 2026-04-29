---
description: Paginated collection of actors
layout: schema
name: ActorCollection
properties_list:
- description: Array of actor records
  name: results
  type: array
- description: Pagination information for list responses.
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-conversations-actor-collection-schema.json
slug: hubspot-conversations-actor-collection
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Paginated collection of actors\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of actor records\",\n      \"example\": [\n        {\n          \"id\": \"actor_101\",\n          \"actorId\": \"actor_101\",\n          \"name\": \"John Customer\",\n          \"email\": \"john@example.com\",\n          \"type\": \"VISITOR\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a participant in a conversation (visitor, agent, or bot).\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the actor\",\n            \"example\": \"actor_101\"\n          },\n          \"actorId\": {\n            \"type\": \"string\",\n            \"description\": \"Actor ID reference\",\n            \"example\": \"actor_101\"\n          },\n          \"name\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"Display name of the actor\",\n            \"example\": \"John Customer\"\n          },\n          \"email\": {\n            \"type\": \"string\",\n            \"description\": \"Email address of the actor\",\n            \"format\": \"email\",\n            \"example\": \"john@example.com\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Type of actor (e.g., VISITOR, AGENT, BOT)\",\n            \"example\": \"VISITOR\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ]\n      }\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information for list responses.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination cursor information for retrieving the next page.\",\n          \"properties\": {\n            \"after\": {\n      \
  \        \"type\": \"string\",\n              \"description\": \"Cursor token for the next page\",\n              \"example\": \"NTI1Cg%3D%3D\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"API link to the next page\",\n              \"example\": \"/conversations/v3/conversations/inboxes?after=NTI1Cg%3D%3D\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActorCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-conversations-actor-collection-schema.json
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
title: ActorCollection
---
