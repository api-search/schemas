---
description: Properties that can be updated on an existing group.
layout: schema
name: GroupUpdate
properties_list:
- description: ''
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: mailNickname
  type: string
- description: ''
  name: visibility
  type: string
- description: ''
  name: membershipRule
  type: string
- description: ''
  name: membershipRuleProcessingState
  type: string
- description: ''
  name: preferredLanguage
  type: string
- description: ''
  name: classification
  type: string
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/microsoft-graph-identity-group-update-schema.json
slug: microsoft-graph-identity-group-update
source_filename: microsoft-graph-identity-group-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Properties that can be updated on an existing group.\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\"\n    },\n    \"visibility\": {\n      \"type\": \"string\"\n    },\n    \"membershipRule\": {\n      \"type\": \"string\"\n    },\n    \"membershipRuleProcessingState\": {\n      \"type\": \"string\"\n    },\n    \"preferredLanguage\": {\n      \"type\": \"string\"\n    },\n    \"classification\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-group-update-schema.json
tags:
- Authentication
- Authorization
- Identity
- Microsoft
- Microsoft Entra
- OAuth
- OpenID Connect
- SAML
- SCIM
- Single Sign-On
- Zero Trust
title: GroupUpdate
---
