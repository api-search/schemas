---
description: A client application registered in a Keycloak realm for authentication.
layout: schema
name: Client
properties_list:
- description: The unique identifier of the client.
  name: id
  type: string
- description: The client identifier used in authentication flows.
  name: clientId
  type: string
- description: The display name of the client.
  name: name
  type: string
- description: A description of the client.
  name: description
  type: string
- description: Whether the client is enabled.
  name: enabled
  type: boolean
- description: The authentication protocol.
  name: protocol
  type: string
- description: Whether the client is public (no client secret).
  name: publicClient
  type: boolean
- description: The root URL of the client application.
  name: rootUrl
  type: string
- description: Allowed redirect URIs after authentication.
  name: redirectUris
  type: array
- description: Allowed web origins for CORS.
  name: webOrigins
  type: array
- description: Whether service accounts are enabled.
  name: serviceAccountsEnabled
  type: boolean
- description: Whether authorization services are enabled.
  name: authorizationServicesEnabled
  type: boolean
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-keycloak-admin-client-schema.json
slug: red-hat-keycloak-admin-client
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Client\",\n  \"type\": \"object\",\n  \"description\": \"A client application registered in a Keycloak realm for authentication.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the client.\"\n    },\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"The client identifier used in authentication flows.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the client.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the client.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the client is enabled.\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"The authentication protocol.\"\n    },\n    \"publicClient\": {\n     \
  \ \"type\": \"boolean\",\n      \"description\": \"Whether the client is public (no client secret).\"\n    },\n    \"rootUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The root URL of the client application.\"\n    },\n    \"redirectUris\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed redirect URIs after authentication.\"\n    },\n    \"webOrigins\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed web origins for CORS.\"\n    },\n    \"serviceAccountsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether service accounts are enabled.\"\n    },\n    \"authorizationServicesEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether authorization services are enabled.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-keycloak-admin-client-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Client
---
