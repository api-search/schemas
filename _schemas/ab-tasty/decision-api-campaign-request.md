---
description: CampaignRequest schema from AB Tasty Decision API
layout: schema
name: CampaignRequest
properties_list:
- description: Unique identifier for the application user or website visitor
  name: visitor_id
  type: string
- description: Identifier for anonymous visitors (e.g., session ID)
  name: anonymous_id
  type: string
- description: JSON object of key-value pairs describing the user and device context
  name: context
  type: object
- description: Determines if visitor has consented to GDPR rules
  name: visitor_consent
  type: boolean
- description: Determines whether a CAMPAIGN hit should be automatically sent
  name: trigger_hit
  type: boolean
- description: Groups visitors to receive the same variation assignment
  name: decision_group
  type: string
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-campaign-request-schema.json
slug: decision-api-campaign-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-request-schema.json\",\n  \"title\": \"CampaignRequest\",\n  \"description\": \"CampaignRequest schema from AB Tasty Decision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"visitor_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the application user or website visitor\",\n      \"example\": \"user123\"\n    },\n    \"anonymous_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for anonymous visitors (e.g., session ID)\",\n      \"example\": \"session_xyz\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"JSON object of key-value pairs describing the user and device context\",\n      \"additionalProperties\": true,\n      \"example\": {\n        \"device\": \"mobile\",\n        \"platform\"\
  : \"ios\",\n        \"subscription_level\": \"premium\"\n      }\n    },\n    \"visitor_consent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Determines if visitor has consented to GDPR rules\",\n      \"default\": true\n    },\n    \"trigger_hit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Determines whether a CAMPAIGN hit should be automatically sent\",\n      \"default\": true\n    },\n    \"decision_group\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Groups visitors to receive the same variation assignment\",\n      \"example\": \"VIP_users\"\n    }\n  },\n  \"required\": [\n    \"visitor_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-campaign-request-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: CampaignRequest
---
