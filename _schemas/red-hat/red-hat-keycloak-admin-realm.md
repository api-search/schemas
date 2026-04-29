---
description: A Keycloak realm representing an isolated tenant for identity management.
layout: schema
name: Realm
properties_list:
- description: The unique identifier of the realm.
  name: id
  type: string
- description: The name of the realm.
  name: realm
  type: string
- description: The display name of the realm.
  name: displayName
  type: string
- description: Whether the realm is enabled.
  name: enabled
  type: boolean
- description: Whether user self-registration is allowed.
  name: registrationAllowed
  type: boolean
- description: Whether users can log in with their email address.
  name: loginWithEmailAllowed
  type: boolean
- description: Whether duplicate emails are allowed.
  name: duplicateEmailsAllowed
  type: boolean
- description: Whether password reset is enabled.
  name: resetPasswordAllowed
  type: boolean
- description: The SSL requirement policy.
  name: sslRequired
  type: string
- description: The access token lifespan in seconds.
  name: accessTokenLifespan
  type: integer
- description: The SSO session idle timeout in seconds.
  name: ssoSessionIdleTimeout
  type: integer
- description: The maximum SSO session lifespan in seconds.
  name: ssoSessionMaxLifespan
  type: integer
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-keycloak-admin-realm-schema.json
slug: red-hat-keycloak-admin-realm
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Realm\",\n  \"type\": \"object\",\n  \"description\": \"A Keycloak realm representing an isolated tenant for identity management.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the realm.\"\n    },\n    \"realm\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the realm.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the realm.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the realm is enabled.\"\n    },\n    \"registrationAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether user self-registration is allowed.\"\n    },\n    \"loginWithEmailAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether users can log in with their email address.\"\n    },\n\
  \    \"duplicateEmailsAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether duplicate emails are allowed.\"\n    },\n    \"resetPasswordAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether password reset is enabled.\"\n    },\n    \"sslRequired\": {\n      \"type\": \"string\",\n      \"description\": \"The SSL requirement policy.\"\n    },\n    \"accessTokenLifespan\": {\n      \"type\": \"integer\",\n      \"description\": \"The access token lifespan in seconds.\"\n    },\n    \"ssoSessionIdleTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"The SSO session idle timeout in seconds.\"\n    },\n    \"ssoSessionMaxLifespan\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum SSO session lifespan in seconds.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-keycloak-admin-realm-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Realm
---
