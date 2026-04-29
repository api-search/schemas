---
description: user-response from GitHub API
layout: schema
name: user-response
properties_list:
- description: The URIs that are used to indicate the namespaces of the SCIM schemas.
  name: schemas
  type: array
- description: A unique identifier for the resource as defined by the provisioning client.
  name: externalId
  type: string
- description: Whether the user active in the IdP.
  name: active
  type: boolean
- description: The username for the user.
  name: userName
  type: string
- description: ''
  name: name
  type: object
- description: A human-readable name for the user.
  name: displayName
  type: string
- description: ''
  name: emails
  type: object
- description: ''
  name: roles
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-scim-user-response-schema.json
slug: github-scim-user-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-scim-user-response-schema.json\",\n  \"title\": \"user-response\",\n  \"description\": \"user-response from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\",\n      \"description\": \"The URIs that are used to indicate the namespaces of the SCIM schemas.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"urn:ietf:params:scim:schemas:core:2.0:User\"\n        ]\n      },\n      \"example\": [\n        \"urn:ietf:params:scim:schemas:core:2.0:User\"\n      ]\n    },\n    \"externalId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the resource as defined by the provisioning client.\",\n      \"example\": \"E012345\",\n      \"nullable\": true\n    },\n    \"active\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Whether the user active in the IdP.\",\n      \"example\": true\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"The username for the user.\",\n      \"example\": \"E012345\"\n    },\n    \"name\": {\n      \"$ref\": \"#/components/schemas/user-name-response\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name for the user.\",\n      \"example\": \"Mona Lisa\",\n      \"nullable\": true\n    },\n    \"emails\": {\n      \"$ref\": \"#/components/schemas/user-emails-response\"\n    },\n    \"roles\": {\n      \"$ref\": \"#/components/schemas/user-role\"\n    }\n  },\n  \"required\": [\n    \"schemas\",\n    \"active\",\n    \"emails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-scim-user-response-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: user-response
---
