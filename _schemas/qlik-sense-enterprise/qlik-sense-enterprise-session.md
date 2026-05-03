---
description: A proxy session represents an authenticated user connection managed by the Qlik Sense Proxy Service. Sessions track user identity, activity timestamps, and session attributes including roles and group memberships.
layout: schema
name: Qlik Sense Proxy Session
properties_list:
- description: Unique session identifier
  name: sessionId
  type: string
- description: Name of the user directory the session user belongs to
  name: userDirectory
  type: string
- description: User identifier within the user directory
  name: userId
  type: string
- description: Display name of the session user
  name: userName
  type: string
- description: ISO 8601 timestamp when the session was created
  name: sessionStart
  type: string
- description: ISO 8601 timestamp of the last activity on this session
  name: lastActive
  type: string
- description: Session attributes passed from the authentication source, including roles and group memberships
  name: attributes
  type: array
provider_name: Qlik Sense Enterprise
provider_slug: qlik-sense-enterprise
schema_file: json-schema/qlik-sense-enterprise-session-schema.json
slug: qlik-sense-enterprise-session
source_filename: qlik-sense-enterprise-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api.dev/qlik-sense-enterprise/session.json\",\n  \"title\": \"Qlik Sense Proxy Session\",\n  \"description\": \"A proxy session represents an authenticated user connection managed by the Qlik Sense Proxy Service. Sessions track user identity, activity timestamps, and session attributes including roles and group memberships.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique session identifier\"\n    },\n    \"userDirectory\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the user directory the session user belongs to\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"User identifier within the user directory\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the session\
  \ user\"\n    },\n    \"sessionStart\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the session was created\"\n    },\n    \"lastActive\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the last activity on this session\"\n    },\n    \"attributes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SessionAttribute\"\n      },\n      \"description\": \"Session attributes passed from the authentication source, including roles and group memberships\"\n    }\n  },\n  \"$defs\": {\n    \"SessionAttribute\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value attribute associated with a session\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Attribute name (e.g., group, role)\"\n        },\n        \"values\": {\n          \"type\": \"array\",\n \
  \         \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Attribute values\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/json-schema/qlik-sense-enterprise-session-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Enterprise
- REST API
title: Qlik Sense Proxy Session
---
