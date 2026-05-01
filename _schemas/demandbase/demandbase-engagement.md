---
description: Represents account-level engagement data in Demandbase, including engagement scores across channels, activity counts, and trend indicators for ABM measurement.
layout: schema
name: Demandbase Account Engagement
properties_list:
- description: Demandbase account identifier
  name: account_id
  type: string
- description: Company name
  name: company_name
  type: string
- description: Overall engagement score (0-100)
  name: engagement_score
  type: number
- description: Engagement trend direction
  name: engagement_trend
  type: string
- description: Web channel engagement score
  name: web_engagement
  type: number
- description: Email channel engagement score
  name: email_engagement
  type: number
- description: Advertising channel engagement score
  name: ad_engagement
  type: number
- description: Timestamp of most recent activity
  name: last_activity_date
  type: string
- description: Total number of tracked activities
  name: total_activities
  type: integer
- description: Overall intent signal strength
  name: intent_strength
  type: string
- description: Estimated buying journey stage
  name: buying_stage
  type: string
provider_name: Demandbase
provider_slug: demandbase
schema_file: json-schema/demandbase-engagement-schema.json
slug: demandbase-engagement
source_filename: demandbase-engagement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.demandbase.com/schemas/demandbase/engagement.json\",\n  \"title\": \"Demandbase Account Engagement\",\n  \"description\": \"Represents account-level engagement data in Demandbase, including engagement scores across channels, activity counts, and trend indicators for ABM measurement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account_id\": {\n      \"type\": \"string\",\n      \"description\": \"Demandbase account identifier\"\n    },\n    \"company_name\": {\n      \"type\": \"string\",\n      \"description\": \"Company name\"\n    },\n    \"engagement_score\": {\n      \"type\": \"number\",\n      \"description\": \"Overall engagement score (0-100)\"\n    },\n    \"engagement_trend\": {\n      \"type\": \"string\",\n      \"enum\": [\"increasing\", \"stable\", \"decreasing\"],\n      \"description\": \"Engagement trend direction\"\n    },\n    \"web_engagement\": {\n\
  \      \"type\": \"number\",\n      \"description\": \"Web channel engagement score\"\n    },\n    \"email_engagement\": {\n      \"type\": \"number\",\n      \"description\": \"Email channel engagement score\"\n    },\n    \"ad_engagement\": {\n      \"type\": \"number\",\n      \"description\": \"Advertising channel engagement score\"\n    },\n    \"last_activity_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of most recent activity\"\n    },\n    \"total_activities\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of tracked activities\"\n    },\n    \"intent_strength\": {\n      \"type\": \"string\",\n      \"enum\": [\"high\", \"medium\", \"low\"],\n      \"description\": \"Overall intent signal strength\"\n    },\n    \"buying_stage\": {\n      \"type\": \"string\",\n      \"enum\": [\"awareness\", \"consideration\", \"decision\", \"purchase\"],\n      \"description\": \"Estimated buying journey\
  \ stage\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/json-schema/demandbase-engagement-schema.json
tags:
- Account-Based Marketing
- Advertising
- AI Agents
- B2B Marketing
- Data Enrichment
- Intent Data
- Personalization
- Sales Intelligence
title: Demandbase Account Engagement
---
