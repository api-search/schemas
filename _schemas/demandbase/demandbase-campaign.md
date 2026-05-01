---
description: Represents an advertising campaign in Demandbase for account-based marketing, including budget, targeting, and scheduling information.
layout: schema
name: Demandbase Campaign
properties_list:
- description: Campaign unique identifier
  name: id
  type: string
- description: Campaign name
  name: name
  type: string
- description: Current campaign status
  name: status
  type: string
- description: Total campaign budget in USD
  name: budget
  type: number
- description: Daily budget cap in USD
  name: daily_budget
  type: number
- description: Campaign start date
  name: start_date
  type: string
- description: Campaign end date
  name: end_date
  type: string
- description: Associated audience segment identifier
  name: audience_id
  type: string
- description: Total impressions served
  name: impressions
  type: integer
- description: Total clicks received
  name: clicks
  type: integer
- description: Click-through rate
  name: ctr
  type: number
- description: Total spend in USD
  name: spend
  type: number
- description: Number of unique target accounts reached
  name: accounts_reached
  type: integer
- description: Number of accounts showing engagement
  name: accounts_engaged
  type: integer
- description: Campaign creation timestamp
  name: created_at
  type: string
- description: Last update timestamp
  name: updated_at
  type: string
provider_name: Demandbase
provider_slug: demandbase
schema_file: json-schema/demandbase-campaign-schema.json
slug: demandbase-campaign
source_filename: demandbase-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.demandbase.com/schemas/demandbase/campaign.json\",\n  \"title\": \"Demandbase Campaign\",\n  \"description\": \"Represents an advertising campaign in Demandbase for account-based marketing, including budget, targeting, and scheduling information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign unique identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign name\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"paused\", \"completed\", \"draft\"],\n      \"description\": \"Current campaign status\"\n    },\n    \"budget\": {\n      \"type\": \"number\",\n      \"description\": \"Total campaign budget in USD\"\n    },\n    \"daily_budget\": {\n      \"type\": \"number\",\n      \"description\": \"Daily budget cap in USD\"\
  \n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Campaign start date\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Campaign end date\"\n    },\n    \"audience_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated audience segment identifier\"\n    },\n    \"impressions\": {\n      \"type\": \"integer\",\n      \"description\": \"Total impressions served\"\n    },\n    \"clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"Total clicks received\"\n    },\n    \"ctr\": {\n      \"type\": \"number\",\n      \"description\": \"Click-through rate\"\n    },\n    \"spend\": {\n      \"type\": \"number\",\n      \"description\": \"Total spend in USD\"\n    },\n    \"accounts_reached\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of unique target accounts reached\"\n    },\n    \"accounts_engaged\": {\n  \
  \    \"type\": \"integer\",\n      \"description\": \"Number of accounts showing engagement\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Campaign creation timestamp\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/json-schema/demandbase-campaign-schema.json
tags:
- Account-Based Marketing
- Advertising
- AI Agents
- B2B Marketing
- Data Enrichment
- Intent Data
- Personalization
- Sales Intelligence
title: Demandbase Campaign
---
