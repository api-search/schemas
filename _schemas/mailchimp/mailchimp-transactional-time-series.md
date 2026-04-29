---
description: An hourly time series data point with sending statistics.
layout: schema
name: TimeSeries
properties_list:
- description: The hour this data point covers (UTC).
  name: time
  type: string
- description: Number of messages sent.
  name: sent
  type: integer
- description: Number of hard bounces.
  name: hard_bounces
  type: integer
- description: Number of soft bounces.
  name: soft_bounces
  type: integer
- description: Number of rejects.
  name: rejects
  type: integer
- description: Number of spam complaints.
  name: complaints
  type: integer
- description: Number of unsubscribes.
  name: unsubs
  type: integer
- description: Number of opens.
  name: opens
  type: integer
- description: Number of unique opens.
  name: unique_opens
  type: integer
- description: Number of clicks.
  name: clicks
  type: integer
- description: Number of unique clicks.
  name: unique_clicks
  type: integer
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-time-series-schema.json
slug: mailchimp-transactional-time-series
source_filename: mailchimp-transactional-time-series-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeSeries\",\n  \"type\": \"object\",\n  \"description\": \"An hourly time series data point with sending statistics.\",\n  \"properties\": {\n    \"time\": {\n      \"type\": \"string\",\n      \"description\": \"The hour this data point covers (UTC).\"\n    },\n    \"sent\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of messages sent.\"\n    },\n    \"hard_bounces\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of hard bounces.\"\n    },\n    \"soft_bounces\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of soft bounces.\"\n    },\n    \"rejects\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rejects.\"\n    },\n    \"complaints\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of spam complaints.\"\n    },\n    \"unsubs\": {\n      \"type\": \"integer\",\n      \"description\": \"Number\
  \ of unsubscribes.\"\n    },\n    \"opens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of opens.\"\n    },\n    \"unique_opens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of unique opens.\"\n    },\n    \"clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of clicks.\"\n    },\n    \"unique_clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of unique clicks.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-time-series-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: TimeSeries
---
