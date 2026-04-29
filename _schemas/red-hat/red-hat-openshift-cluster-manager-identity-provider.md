---
description: Represents an identity provider configured for cluster authentication.
layout: schema
name: IdentityProvider
properties_list:
- description: The unique identifier of the identity provider.
  name: id
  type: string
- description: The display name of the identity provider.
  name: name
  type: string
- description: The type of identity provider.
  name: type
  type: string
- description: The method used to map identities to users.
  name: mapping_method
  type: string
- description: GitHub-specific identity provider configuration.
  name: github
  type: object
- description: LDAP-specific identity provider configuration.
  name: ldap
  type: object
- description: OpenID Connect identity provider configuration.
  name: openid
  type: object
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-openshift-cluster-manager-identity-provider-schema.json
slug: red-hat-openshift-cluster-manager-identity-provider
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IdentityProvider\",\n  \"type\": \"object\",\n  \"description\": \"Represents an identity provider configured for cluster authentication.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the identity provider.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the identity provider.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of identity provider.\"\n    },\n    \"mapping_method\": {\n      \"type\": \"string\",\n      \"description\": \"The method used to map identities to users.\"\n    },\n    \"github\": {\n      \"type\": \"object\",\n      \"description\": \"GitHub-specific identity provider configuration.\"\n    },\n    \"ldap\": {\n      \"type\": \"object\",\n      \"description\": \"LDAP-specific identity provider configuration.\"\
  \n    },\n    \"openid\": {\n      \"type\": \"object\",\n      \"description\": \"OpenID Connect identity provider configuration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-openshift-cluster-manager-identity-provider-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: IdentityProvider
---
