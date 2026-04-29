---
description: An external identity provider configured for federated authentication.
layout: schema
name: IdentityProviderRepresentation
properties_list:
- description: The unique alias for the identity provider.
  name: alias
  type: string
- description: The display name of the identity provider.
  name: displayName
  type: string
- description: The provider type identifier.
  name: providerId
  type: string
- description: Whether the identity provider is enabled.
  name: enabled
  type: boolean
- description: Provider-specific configuration.
  name: config
  type: object
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-keycloak-admin-identity-provider-representation-schema.json
slug: red-hat-keycloak-admin-identity-provider-representation
source_filename: red-hat-keycloak-admin-identity-provider-representation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IdentityProviderRepresentation\",\n  \"type\": \"object\",\n  \"description\": \"An external identity provider configured for federated authentication.\",\n  \"properties\": {\n    \"alias\": {\n      \"type\": \"string\",\n      \"description\": \"The unique alias for the identity provider.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the identity provider.\"\n    },\n    \"providerId\": {\n      \"type\": \"string\",\n      \"description\": \"The provider type identifier.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the identity provider is enabled.\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Provider-specific configuration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-keycloak-admin-identity-provider-representation-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: IdentityProviderRepresentation
---
