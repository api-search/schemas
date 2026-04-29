---
description: ''
layout: schema
name: Body_token_auth_token_post
properties_list:
- description: ''
  name: grant_type
  type: object
- description: ''
  name: username
  type: string
- description: ''
  name: password
  type: string
- description: ''
  name: scope
  type: string
- description: ''
  name: client_id
  type: object
- description: ''
  name: client_secret
  type: object
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-weather-service-body-token-auth-token-post-schema.json
slug: agstack-openagri-weather-service-body-token-auth-token-post
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/Body_token_auth_token_post.json\",\n  \"title\": \"Body_token_auth_token_post\",\n  \"properties\": {\n    \"grant_type\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"password\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Grant Type\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"title\": \"Username\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"title\": \"Password\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"title\": \"Scope\",\n      \"default\": \"\"\n    },\n    \"client_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Client Id\"\n    },\n    \"client_secret\": {\n      \"anyOf\": [\n   \
  \     {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Client Secret\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"username\",\n    \"password\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-weather-service-body-token-auth-token-post-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: Body_token_auth_token_post
---
