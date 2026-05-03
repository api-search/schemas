---
description: A web application protected by SafeLine WAF reverse proxy.
layout: schema
name: SafeLine Protected Website
properties_list:
- description: Unique website identifier
  name: id
  type: integer
- description: Friendly name for the protected website
  name: name
  type: string
- description: Backend server address (host:port or IP:port)
  name: upstream
  type: string
- description: Listener ports for the reverse proxy
  name: ports
  type: array
- description: Whether WAF protection is enabled
  name: enabled
  type: boolean
- description: Applied security policy group ID
  name: policy_group_id
  type: integer
- description: SSL certificate ID for HTTPS
  name: ssl_id
  type: integer
- description: Website creation timestamp
  name: create_time
  type: string
- description: Optional description or notes
  name: comment
  type: string
provider_name: SafeLine
provider_slug: safeline
schema_file: json-schema/safeline-website-schema.json
slug: safeline-website
source_filename: safeline-website-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/safeline/main/json-schema/safeline-website-schema.json\",\n  \"title\": \"SafeLine Protected Website\",\n  \"description\": \"A web application protected by SafeLine WAF reverse proxy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique website identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Friendly name for the protected website\"\n    },\n    \"upstream\": {\n      \"type\": \"string\",\n      \"description\": \"Backend server address (host:port or IP:port)\",\n      \"example\": \"192.168.1.100:8080\"\n    },\n    \"ports\": {\n      \"type\": \"array\",\n      \"description\": \"Listener ports for the reverse proxy\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"port\": {\n   \
  \         \"type\": \"integer\",\n            \"description\": \"Port number\"\n          },\n          \"protocol\": {\n            \"type\": \"string\",\n            \"enum\": [\"http\", \"https\"],\n            \"description\": \"Protocol type\"\n          }\n        },\n        \"required\": [\"port\", \"protocol\"]\n      }\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether WAF protection is enabled\"\n    },\n    \"policy_group_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Applied security policy group ID\"\n    },\n    \"ssl_id\": {\n      \"type\": \"integer\",\n      \"description\": \"SSL certificate ID for HTTPS\"\n    },\n    \"create_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Website creation timestamp\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description or notes\"\n    }\n  },\n  \"required\": [\"id\", \"name\"\
  , \"upstream\", \"ports\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/safeline/refs/heads/main/json-schema/safeline-website-schema.json
tags:
- Proxy
- WAF
- Security
- Open Source
- Reverse Proxy
- API Gateway
title: SafeLine Protected Website
---
