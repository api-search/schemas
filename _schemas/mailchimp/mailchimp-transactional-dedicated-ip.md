---
description: Information about a dedicated IP address.
layout: schema
name: DedicatedIP
properties_list:
- description: The dedicated IP address.
  name: ip
  type: string
- description: When the IP was provisioned.
  name: created_at
  type: string
- description: The IP pool this address belongs to.
  name: pool
  type: string
- description: The reverse DNS domain for the IP.
  name: domain
  type: string
- description: Custom DNS settings for the IP.
  name: custom_dns
  type: object
- description: IP warmup status.
  name: warmup
  type: object
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-dedicated-ip-schema.json
slug: mailchimp-transactional-dedicated-ip
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DedicatedIP\",\n  \"type\": \"object\",\n  \"description\": \"Information about a dedicated IP address.\",\n  \"properties\": {\n    \"ip\": {\n      \"type\": \"string\",\n      \"description\": \"The dedicated IP address.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the IP was provisioned.\"\n    },\n    \"pool\": {\n      \"type\": \"string\",\n      \"description\": \"The IP pool this address belongs to.\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The reverse DNS domain for the IP.\"\n    },\n    \"custom_dns\": {\n      \"type\": \"object\",\n      \"description\": \"Custom DNS settings for the IP.\"\n    },\n    \"warmup\": {\n      \"type\": \"object\",\n      \"description\": \"IP warmup status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-dedicated-ip-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: DedicatedIP
---
