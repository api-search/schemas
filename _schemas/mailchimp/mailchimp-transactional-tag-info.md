---
description: Information and statistics for a message tag.
layout: schema
name: TagInfo
properties_list:
- description: The tag name.
  name: tag
  type: string
- description: The reputation score for the tag (0-100).
  name: reputation
  type: integer
- description: Total number of messages sent with this tag.
  name: sent
  type: integer
- description: Total hard bounces for messages with this tag.
  name: hard_bounces
  type: integer
- description: Total soft bounces for messages with this tag.
  name: soft_bounces
  type: integer
- description: Total rejects for messages with this tag.
  name: rejects
  type: integer
- description: Total spam complaints for messages with this tag.
  name: complaints
  type: integer
- description: Total unsubscribes for messages with this tag.
  name: unsubs
  type: integer
- description: Total opens for messages with this tag.
  name: opens
  type: integer
- description: Total clicks for messages with this tag.
  name: clicks
  type: integer
- description: Unique opens for messages with this tag.
  name: unique_opens
  type: integer
- description: Unique clicks for messages with this tag.
  name: unique_clicks
  type: integer
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-tag-info-schema.json
slug: mailchimp-transactional-tag-info
source_filename: mailchimp-transactional-tag-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagInfo\",\n  \"type\": \"object\",\n  \"description\": \"Information and statistics for a message tag.\",\n  \"properties\": {\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"The tag name.\"\n    },\n    \"reputation\": {\n      \"type\": \"integer\",\n      \"description\": \"The reputation score for the tag (0-100).\"\n    },\n    \"sent\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of messages sent with this tag.\"\n    },\n    \"hard_bounces\": {\n      \"type\": \"integer\",\n      \"description\": \"Total hard bounces for messages with this tag.\"\n    },\n    \"soft_bounces\": {\n      \"type\": \"integer\",\n      \"description\": \"Total soft bounces for messages with this tag.\"\n    },\n    \"rejects\": {\n      \"type\": \"integer\",\n      \"description\": \"Total rejects for messages with this tag.\"\n    },\n    \"complaints\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Total spam complaints for messages with this tag.\"\n    },\n    \"unsubs\": {\n      \"type\": \"integer\",\n      \"description\": \"Total unsubscribes for messages with this tag.\"\n    },\n    \"opens\": {\n      \"type\": \"integer\",\n      \"description\": \"Total opens for messages with this tag.\"\n    },\n    \"clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"Total clicks for messages with this tag.\"\n    },\n    \"unique_opens\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique opens for messages with this tag.\"\n    },\n    \"unique_clicks\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique clicks for messages with this tag.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-tag-info-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: TagInfo
---
