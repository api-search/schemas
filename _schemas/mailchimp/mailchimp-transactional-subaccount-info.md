---
description: Information about a subaccount.
layout: schema
name: SubaccountInfo
properties_list:
- description: The unique subaccount identifier.
  name: id
  type: string
- description: The display name of the subaccount.
  name: name
  type: string
- description: Notes about the subaccount.
  name: notes
  type: string
- description: The manual hourly quota, if set.
  name: custom_quota
  type: integer
- description: The current status of the subaccount.
  name: status
  type: string
- description: The subaccount sending reputation (0-100).
  name: reputation
  type: integer
- description: When the subaccount was created.
  name: created_at
  type: string
- description: When the subaccount first sent a message.
  name: first_sent_at
  type: string
- description: Messages sent in the last week.
  name: sent_weekly
  type: integer
- description: Messages sent in the last month.
  name: sent_monthly
  type: integer
- description: Total messages sent.
  name: sent_total
  type: integer
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-subaccount-info-schema.json
slug: mailchimp-transactional-subaccount-info
source_filename: mailchimp-transactional-subaccount-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubaccountInfo\",\n  \"type\": \"object\",\n  \"description\": \"Information about a subaccount.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique subaccount identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the subaccount.\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Notes about the subaccount.\"\n    },\n    \"custom_quota\": {\n      \"type\": \"integer\",\n      \"description\": \"The manual hourly quota, if set.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the subaccount.\"\n    },\n    \"reputation\": {\n      \"type\": \"integer\",\n      \"description\": \"The subaccount sending reputation (0-100).\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"\
  description\": \"When the subaccount was created.\"\n    },\n    \"first_sent_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the subaccount first sent a message.\"\n    },\n    \"sent_weekly\": {\n      \"type\": \"integer\",\n      \"description\": \"Messages sent in the last week.\"\n    },\n    \"sent_monthly\": {\n      \"type\": \"integer\",\n      \"description\": \"Messages sent in the last month.\"\n    },\n    \"sent_total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total messages sent.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-subaccount-info-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: SubaccountInfo
---
