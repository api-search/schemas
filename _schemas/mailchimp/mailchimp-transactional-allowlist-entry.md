---
description: An entry in the sending allowlist.
layout: schema
name: AllowlistEntry
properties_list:
- description: The allowlisted email address.
  name: email
  type: string
- description: Details or comment about why the address is allowlisted.
  name: detail
  type: string
- description: When the entry was added to the allowlist.
  name: created_at
  type: string
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-allowlist-entry-schema.json
slug: mailchimp-transactional-allowlist-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AllowlistEntry\",\n  \"type\": \"object\",\n  \"description\": \"An entry in the sending allowlist.\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The allowlisted email address.\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"Details or comment about why the address is allowlisted.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the entry was added to the allowlist.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-allowlist-entry-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: AllowlistEntry
---
