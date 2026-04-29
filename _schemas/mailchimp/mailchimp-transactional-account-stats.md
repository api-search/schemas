---
description: Aggregate sending statistics for a time period.
layout: schema
name: AccountStats
properties_list:
- description: Total messages sent.
  name: sent
  type: integer
- description: Total hard bounces.
  name: hard_bounces
  type: integer
- description: Total soft bounces.
  name: soft_bounces
  type: integer
- description: Total rejections.
  name: rejects
  type: integer
- description: Total spam complaints.
  name: complaints
  type: integer
- description: Total unsubscribes.
  name: unsubs
  type: integer
- description: Total opens.
  name: opens
  type: integer
- description: Unique opens.
  name: unique_opens
  type: integer
- description: Total clicks.
  name: clicks
  type: integer
- description: Unique clicks.
  name: unique_clicks
  type: integer
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-account-stats-schema.json
slug: mailchimp-transactional-account-stats
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountStats\",\n  \"type\": \"object\",\n  \"description\": \"Aggregate sending statistics for a time period.\",\n  \"properties\": {\n    \"sent\": {\n      \"type\": \"integer\",\n      \"description\": \"Total messages sent.\"\n    },\n    \"hard_bounces\": {\n      \"type\": \"integer\",\n      \"description\": \"Total hard bounces.\"\n    },\n    \"soft_bounces\": {\n      \"type\": \"integer\",\n      \"description\": \"Total soft bounces.\"\n    },\n    \"rejects\": {\n      \"type\": \"integer\",\n      \"description\": \"Total rejections.\"\n    },\n    \"complaints\": {\n      \"type\": \"integer\",\n      \"description\": \"Total spam complaints.\"\n    },\n    \"unsubs\": {\n      \"type\": \"integer\",\n      \"description\": \"Total unsubscribes.\"\n    },\n    \"opens\": {\n      \"type\": \"integer\",\n      \"description\": \"Total opens.\"\n    },\n    \"unique_opens\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"Unique opens.\"\n    },\n    \"clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"Total clicks.\"\n    },\n    \"unique_clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique clicks.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-account-stats-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: AccountStats
---
