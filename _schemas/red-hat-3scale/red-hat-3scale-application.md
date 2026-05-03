---
description: Schema for an application in Red Hat 3scale API Management. Applications hold API credentials and are subscribed to application plans.
layout: schema
name: Red Hat 3scale Application
properties_list:
- description: Unique application identifier
  name: id
  type: integer
- description: Application creation timestamp
  name: created_at
  type: string
- description: Application last updated timestamp
  name: updated_at
  type: string
- description: Application state
  name: state
  type: string
- description: ID of the developer account that owns this application
  name: user_account_id
  type: integer
- description: Application display name
  name: name
  type: string
- description: Application description
  name: description
  type: string
- description: API key credential for API key authentication mode
  name: user_key
  type: string
- description: The application plan this application is subscribed to
  name: plan
  type: object
provider_name: Red Hat 3scale
provider_slug: red-hat-3scale
schema_file: json-schema/red-hat-3scale-application-schema.json
slug: red-hat-3scale-application
source_filename: red-hat-3scale-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/red-hat-3scale/json-schema/red-hat-3scale-application-schema.json\",\n  \"title\": \"Red Hat 3scale Application\",\n  \"description\": \"Schema for an application in Red Hat 3scale API Management. Applications hold API credentials and are subscribed to application plans.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"state\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique application identifier\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Application creation timestamp\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Application last updated timestamp\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"live\", \"suspended\"\
  ],\n      \"description\": \"Application state\"\n    },\n    \"user_account_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the developer account that owns this application\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application display name\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Application description\"\n    },\n    \"user_key\": {\n      \"type\": \"string\",\n      \"description\": \"API key credential for API key authentication mode\"\n    },\n    \"plan\": {\n      \"type\": \"object\",\n      \"description\": \"The application plan this application is subscribed to\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"system_name\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/json-schema/red-hat-3scale-application-schema.json
tags:
- API Gateway
- API Management
- Developer Portal
- Enterprise
- Red Hat
title: Red Hat 3scale Application
---
