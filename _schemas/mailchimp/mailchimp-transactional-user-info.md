---
description: Account-level information for the authenticated Mandrill user.
layout: schema
name: UserInfo
properties_list:
- description: The account username.
  name: username
  type: string
- description: When the account was created.
  name: created_at
  type: string
- description: A unique public identifier for the account.
  name: public_id
  type: string
- description: The account sending reputation (0-100).
  name: reputation
  type: integer
- description: The hourly email sending quota.
  name: hourly_quota
  type: integer
- description: The number of messages in the send queue.
  name: backlog
  type: integer
- description: Account-level sending statistics.
  name: stats
  type: object
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-user-info-schema.json
slug: mailchimp-transactional-user-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserInfo\",\n  \"type\": \"object\",\n  \"description\": \"Account-level information for the authenticated Mandrill user.\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The account username.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the account was created.\"\n    },\n    \"public_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique public identifier for the account.\"\n    },\n    \"reputation\": {\n      \"type\": \"integer\",\n      \"description\": \"The account sending reputation (0-100).\"\n    },\n    \"hourly_quota\": {\n      \"type\": \"integer\",\n      \"description\": \"The hourly email sending quota.\"\n    },\n    \"backlog\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of messages in the send queue.\"\n    },\n    \"stats\": {\n \
  \     \"type\": \"object\",\n      \"description\": \"Account-level sending statistics.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-user-info-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: UserInfo
---
