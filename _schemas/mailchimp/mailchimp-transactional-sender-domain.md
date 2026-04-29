---
description: Information about a configured sender domain.
layout: schema
name: SenderDomain
properties_list:
- description: The domain name.
  name: domain
  type: string
- description: When the domain was added.
  name: created_at
  type: string
- description: When the domain settings were last tested.
  name: last_tested_at
  type: string
- description: SPF verification details.
  name: spf
  type: object
- description: DKIM verification details.
  name: dkim
  type: object
- description: When the domain ownership was verified.
  name: verified_at
  type: string
- description: Whether the domain can be used for DKIM signing.
  name: valid_signing
  type: boolean
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-sender-domain-schema.json
slug: mailchimp-transactional-sender-domain
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SenderDomain\",\n  \"type\": \"object\",\n  \"description\": \"Information about a configured sender domain.\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain name.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the domain was added.\"\n    },\n    \"last_tested_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the domain settings were last tested.\"\n    },\n    \"spf\": {\n      \"type\": \"object\",\n      \"description\": \"SPF verification details.\"\n    },\n    \"dkim\": {\n      \"type\": \"object\",\n      \"description\": \"DKIM verification details.\"\n    },\n    \"verified_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the domain ownership was verified.\"\n    },\n    \"valid_signing\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the domain can be used for DKIM signing.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-sender-domain-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: SenderDomain
---
