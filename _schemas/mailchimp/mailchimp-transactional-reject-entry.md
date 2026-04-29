---
description: An entry in the rejection blacklist.
layout: schema
name: RejectEntry
properties_list:
- description: The rejected email address.
  name: email
  type: string
- description: The reason the address is on the blacklist.
  name: reason
  type: string
- description: Extended details about the rejection.
  name: detail
  type: string
- description: When the entry was added to the blacklist.
  name: created_at
  type: string
- description: When the last event occurred for this address.
  name: last_event_at
  type: string
- description: When the rejection expires (if applicable).
  name: expires_at
  type: string
- description: Whether the rejection has expired.
  name: expired
  type: boolean
- description: The subaccount this rejection applies to, if any.
  name: subaccount
  type: string
- description: Sender statistics associated with the rejection.
  name: sender
  type: object
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-reject-entry-schema.json
slug: mailchimp-transactional-reject-entry
source_filename: mailchimp-transactional-reject-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RejectEntry\",\n  \"type\": \"object\",\n  \"description\": \"An entry in the rejection blacklist.\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The rejected email address.\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the address is on the blacklist.\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"Extended details about the rejection.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the entry was added to the blacklist.\"\n    },\n    \"last_event_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the last event occurred for this address.\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the rejection expires (if applicable).\"\n    },\n    \"expired\": {\n\
  \      \"type\": \"boolean\",\n      \"description\": \"Whether the rejection has expired.\"\n    },\n    \"subaccount\": {\n      \"type\": \"string\",\n      \"description\": \"The subaccount this rejection applies to, if any.\"\n    },\n    \"sender\": {\n      \"type\": \"object\",\n      \"description\": \"Sender statistics associated with the rejection.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-reject-entry-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: RejectEntry
---
