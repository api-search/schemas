---
description: An authenticated session in ForgeRock Access Management. Sessions are created upon successful authentication and tracked via SSO tokens (iPlanetDirectoryPro cookies).
layout: schema
name: ForgeRock Session
properties_list:
- description: The SSO token identifier for this session
  name: tokenId
  type: string
- description: Username of the session owner
  name: username
  type: string
- description: Universal identifier for the session owner (e.g., id=user,ou=user,dc=example,dc=com)
  name: universalId
  type: string
- description: The realm in which the session was created
  name: realm
  type: string
- description: Most recent time the session was accessed
  name: latestAccessTime
  type: string
- description: Time at which the session will expire due to inactivity
  name: maxIdleExpirationTime
  type: string
- description: Absolute maximum session expiration time regardless of activity
  name: maxSessionExpirationTime
  type: string
- description: Custom session properties
  name: properties
  type: object
- description: Whether the session is currently valid
  name: valid
  type: boolean
- description: Type of session
  name: sessionType
  type: string
provider_name: ForgeRock
provider_slug: forgerock
schema_file: json-schema/forgerock-session-schema.json
slug: forgerock-session
source_filename: forgerock-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.forgerock.com/session\",\n  \"title\": \"ForgeRock Session\",\n  \"description\": \"An authenticated session in ForgeRock Access Management. Sessions are created upon successful authentication and tracked via SSO tokens (iPlanetDirectoryPro cookies).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tokenId\": {\n      \"type\": \"string\",\n      \"description\": \"The SSO token identifier for this session\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the session owner\"\n    },\n    \"universalId\": {\n      \"type\": \"string\",\n      \"description\": \"Universal identifier for the session owner (e.g., id=user,ou=user,dc=example,dc=com)\"\n    },\n    \"realm\": {\n      \"type\": \"string\",\n      \"description\": \"The realm in which the session was created\"\n    },\n    \"latestAccessTime\": {\n      \"type\": \"\
  string\",\n      \"format\": \"date-time\",\n      \"description\": \"Most recent time the session was accessed\"\n    },\n    \"maxIdleExpirationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time at which the session will expire due to inactivity\"\n    },\n    \"maxSessionExpirationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Absolute maximum session expiration time regardless of activity\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Custom session properties\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the session is currently valid\"\n    },\n    \"sessionType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of session\",\n      \"enum\": [\"user\", \"stateless\"]\n    }\n  },\n  \"required\": [\"tokenId\"\
  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/json-schema/forgerock-session-schema.json
tags:
- Access Management
- Authentication
- Authorization
- Identity Governance
- Identity Management
- OAuth
- OpenID Connect
title: ForgeRock Session
---
