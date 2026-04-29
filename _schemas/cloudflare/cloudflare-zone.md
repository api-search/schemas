---
description: A zone object from the Cloudflare API, representing a domain and its associated configuration managed through Cloudflare's DNS and proxy services.
layout: schema
name: Cloudflare Zone
properties_list:
- description: The unique identifier of the zone.
  name: id
  type: string
- description: The domain name of the zone.
  name: name
  type: string
- description: The status of the zone.
  name: status
  type: string
- description: Whether the zone is paused, meaning Cloudflare will not proxy traffic.
  name: paused
  type: boolean
- description: The type of zone configuration.
  name: type
  type: string
- description: Seconds remaining in development mode. Zero means development mode is off.
  name: development_mode
  type: integer
- description: Cloudflare-assigned nameservers for the zone.
  name: name_servers
  type: array
- description: The original nameservers before moving to Cloudflare.
  name: original_name_servers
  type: array
- description: The original domain registrar.
  name: original_registrar
  type: string
- description: The original DNS host.
  name: original_dnshost
  type: string
- description: The account that owns the zone.
  name: account
  type: object
- description: The owner of the zone.
  name: owner
  type: object
- description: The plan associated with the zone.
  name: plan
  type: object
- description: Available permissions on the zone.
  name: permissions
  type: array
- description: When the zone was activated on Cloudflare.
  name: activated_on
  type:
  - string
  - 'null'
- description: When the zone was created.
  name: created_on
  type: string
- description: When the zone was last modified.
  name: modified_on
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-zone-schema.json
slug: cloudflare-zone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-zone-schema.json\",\n  \"title\": \"Cloudflare Zone\",\n  \"description\": \"A zone object from the Cloudflare API, representing a domain and its associated configuration managed through Cloudflare's DNS and proxy services.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the zone.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The domain name of the zone.\",\n      \"format\": \"hostname\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the zone.\",\n      \"enum\": [\"active\", \"pending\", \"initializing\", \"moved\", \"deleted\", \"deactivated\"]\n    },\n    \"paused\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the zone is paused, meaning Cloudflare will not proxy traffic.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of zone configuration.\",\n      \"enum\": [\"full\", \"partial\", \"secondary\"]\n    },\n    \"development_mode\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds remaining in development mode. Zero means development mode is off.\",\n      \"minimum\": 0\n    },\n    \"name_servers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Cloudflare-assigned nameservers for the zone.\"\n    },\n    \"original_name_servers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The original nameservers before moving to Cloudflare.\"\n    },\n    \"original_registrar\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ original domain registrar.\"\n    },\n    \"original_dnshost\": {\n      \"type\": \"string\",\n      \"description\": \"The original DNS host.\"\n    },\n    \"account\": {\n      \"type\": \"object\",\n      \"description\": \"The account that owns the zone.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The account identifier.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The account name.\"\n        }\n      }\n    },\n    \"owner\": {\n      \"type\": \"object\",\n      \"description\": \"The owner of the zone.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The owner identifier.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of owner.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n       \
  \   \"description\": \"The owner email address.\"\n        }\n      }\n    },\n    \"plan\": {\n      \"type\": \"object\",\n      \"description\": \"The plan associated with the zone.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The plan identifier.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The plan name.\"\n        },\n        \"price\": {\n          \"type\": \"number\",\n          \"description\": \"The price of the plan.\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"The currency of the price.\"\n        },\n        \"frequency\": {\n          \"type\": \"string\",\n          \"description\": \"Billing frequency.\",\n          \"enum\": [\"weekly\", \"monthly\", \"quarterly\", \"yearly\"]\n        },\n        \"is_subscribed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the zone\
  \ is subscribed to this plan.\"\n        }\n      }\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Available permissions on the zone.\"\n    },\n    \"activated_on\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the zone was activated on Cloudflare.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the zone was created.\"\n    },\n    \"modified_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the zone was last modified.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-zone-schema.json
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
title: Cloudflare Zone
---
