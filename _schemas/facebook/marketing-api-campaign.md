---
description: An advertising campaign.
layout: schema
name: Campaign
properties_list:
- description: Campaign ID.
  name: id
  type: string
- description: Campaign name.
  name: name
  type: string
- description: Campaign objective.
  name: objective
  type: string
- description: Campaign status.
  name: status
  type: string
- description: Daily budget in cents.
  name: daily_budget
  type: string
- description: Lifetime budget in cents.
  name: lifetime_budget
  type: string
- description: Campaign creation time.
  name: created_time
  type: string
- description: Campaign last update time.
  name: updated_time
  type: string
provider_name: Facebook
provider_slug: facebook
schema_file: json-schema/marketing-api-campaign-schema.json
slug: marketing-api-campaign
source_filename: marketing-api-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/marketing-api-campaign-schema.json\",\n  \"title\": \"Campaign\",\n  \"description\": \"An advertising campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Campaign ID.\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Campaign name.\" },\n    \"objective\": { \"type\": \"string\", \"description\": \"Campaign objective.\" },\n    \"status\": { \"type\": \"string\", \"description\": \"Campaign status.\", \"enum\": [\"ACTIVE\", \"PAUSED\", \"DELETED\", \"ARCHIVED\"] },\n    \"daily_budget\": { \"type\": \"string\", \"description\": \"Daily budget in cents.\" },\n    \"lifetime_budget\": { \"type\": \"string\", \"description\": \"Lifetime budget in cents.\" },\n    \"created_time\": { \"type\": \"string\", \"format\": \"date-time\", \"description\"\
  : \"Campaign creation time.\" },\n    \"updated_time\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Campaign last update time.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/marketing-api-campaign-schema.json
tags:
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
title: Campaign
---
