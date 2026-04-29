---
description: An IP pool grouping dedicated IPs.
layout: schema
name: IPPool
properties_list:
- description: The pool name.
  name: name
  type: string
- description: When the pool was created.
  name: created_at
  type: string
- description: The dedicated IPs in this pool.
  name: ips
  type: array
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-ip-pool-schema.json
slug: mailchimp-transactional-ip-pool
source_filename: mailchimp-transactional-ip-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IPPool\",\n  \"type\": \"object\",\n  \"description\": \"An IP pool grouping dedicated IPs.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The pool name.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the pool was created.\"\n    },\n    \"ips\": {\n      \"type\": \"array\",\n      \"description\": \"The dedicated IPs in this pool.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-ip-pool-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: IPPool
---
