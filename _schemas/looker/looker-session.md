---
description: An active user session
layout: schema
name: Session
properties_list:
- description: Unique session identifier
  name: id
  type: integer
- description: IP address of the session
  name: ip_address
  type: string
- description: Browser used for this session
  name: browser
  type: string
- description: Operating system used for this session
  name: operating_system
  type: string
- description: City from which the session originates
  name: city
  type: string
- description: State from which the session originates
  name: state
  type: string
- description: Country from which the session originates
  name: country
  type: string
- description: Type of credentials used
  name: credentials_type
  type: string
- description: Timestamp when the session was last extended
  name: extended_at
  type: string
- description: Number of times the session has been extended
  name: extended_count
  type: integer
- description: ID of the user being sudo'd as
  name: sudo_user_id
  type: integer
- description: Timestamp when the session was created
  name: created_at
  type: string
- description: Timestamp when the session expires
  name: expires_at
  type: string
- description: Relative URL
  name: url
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-session-schema.json
slug: looker-session
source_filename: looker-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Session\",\n  \"type\": \"object\",\n  \"description\": \"An active user session\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique session identifier\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the session\"\n    },\n    \"browser\": {\n      \"type\": \"string\",\n      \"description\": \"Browser used for this session\"\n    },\n    \"operating_system\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system used for this session\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City from which the session originates\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State from which the session originates\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country from\
  \ which the session originates\"\n    },\n    \"credentials_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of credentials used\"\n    },\n    \"extended_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the session was last extended\"\n    },\n    \"extended_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times the session has been extended\"\n    },\n    \"sudo_user_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the user being sudo'd as\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the session was created\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the session expires\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-session-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: Session
---
