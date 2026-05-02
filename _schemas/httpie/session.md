---
description: Schema representing an HTTPie named session, which persists headers, authentication, and cookies across requests.
layout: schema
name: HTTPie Session
properties_list:
- description: The name of the HTTPie session.
  name: name
  type: string
- description: The host associated with this session.
  name: host
  type: string
- description: Authentication credentials stored in the session.
  name: auth
  type: object
- description: Default headers sent with every request in this session.
  name: headers
  type: object
- description: Cookies stored and sent with requests in this session.
  name: cookies
  type: array
- description: Whether to verify SSL certificates for requests in this session.
  name: verify
  type: boolean
provider_name: HTTPie
provider_slug: httpie
schema_file: json-schema/session.json
slug: session
source_filename: session.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/httpie/refs/heads/main/json-schema/session.json\",\n  \"title\": \"HTTPie Session\",\n  \"description\": \"Schema representing an HTTPie named session, which persists headers, authentication, and cookies across requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the HTTPie session.\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The host associated with this session.\"\n    },\n    \"auth\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication credentials stored in the session.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The authentication type.\",\n          \"enum\": [\"basic\", \"bearer\", \"digest\"]\n        },\n        \"username\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Username for basic or digest authentication.\"\n        },\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"Password for basic or digest authentication.\"\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"Token for bearer authentication.\"\n        }\n      }\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Default headers sent with every request in this session.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"cookies\": {\n      \"type\": \"array\",\n      \"description\": \"Cookies stored and sent with requests in this session.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The cookie name.\"\n          },\n          \"value\": {\n   \
  \         \"type\": \"string\",\n            \"description\": \"The cookie value.\"\n          },\n          \"domain\": {\n            \"type\": \"string\",\n            \"description\": \"The domain the cookie is scoped to.\"\n          },\n          \"path\": {\n            \"type\": \"string\",\n            \"description\": \"The path the cookie is scoped to.\"\n          },\n          \"secure\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the cookie requires HTTPS.\"\n          },\n          \"expires\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The expiration date-time of the cookie.\"\n          }\n        },\n        \"required\": [\"name\", \"value\"]\n      }\n    },\n    \"verify\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to verify SSL certificates for requests in this session.\",\n      \"default\": true\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/httpie/refs/heads/main/json-schema/session.json
tags:
- API Client
- API Testing
- CLI
- Client
- Command Line
- Developer Tools
- HTTP
- Open Source
- Sessions
title: HTTPie Session
---
