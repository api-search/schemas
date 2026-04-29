---
description: A Cloudflare account object representing an organizational entity that owns zones, Workers, and other resources on the Cloudflare platform.
layout: schema
name: Cloudflare Account
properties_list:
- description: The unique identifier of the account.
  name: id
  type: string
- description: The name of the account.
  name: name
  type: string
- description: The type of account.
  name: type
  type: string
- description: Account-level settings.
  name: settings
  type: object
- description: When the account was created.
  name: created_on
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-account-schema.json
slug: cloudflare-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-account-schema.json\",\n  \"title\": \"Cloudflare Account\",\n  \"description\": \"A Cloudflare account object representing an organizational entity that owns zones, Workers, and other resources on the Cloudflare platform.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the account.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the account.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of account.\",\n      \"enum\": [\"standard\", \"enterprise\"]\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"description\": \"Account-level settings.\",\n      \"properties\"\
  : {\n        \"enforce_twofactor\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether two-factor authentication is enforced for all members.\"\n        },\n        \"use_account_custom_ns_by_default\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to use account custom nameservers by default.\"\n        },\n        \"default_nameservers\": {\n          \"type\": \"string\",\n          \"description\": \"The type of default nameservers.\",\n          \"enum\": [\"cloudflare.standard\", \"custom.account\", \"custom.tenant\"]\n        }\n      }\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the account was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-account-schema.json
tags:
- AI Gateway
- API Gateway
- Artificial Intelligence
- CDN
- Cloud
- Containers
- DDoS Protection
- DNS
- Edge
- Edge Computing
- Object Storage
- Platform
- Real-Time Communication
- Security
- Serverless
- Web Performance
title: Cloudflare Account
---
