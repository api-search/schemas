---
description: group-response from GitHub API
layout: schema
name: group-response
properties_list:
- description: The URIs that are used to indicate the namespaces of the SCIM schemas.
  name: schemas
  type: array
- description: A unique identifier for the resource as defined by the provisioning client.
  name: externalId
  type: string
- description: A human-readable name for a security group.
  name: displayName
  type: string
- description: The group members.
  name: members
  type: array
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-scim-group-response-schema.json
slug: github-scim-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-scim-group-response-schema.json\",\n  \"title\": \"group-response\",\n  \"description\": \"group-response from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\",\n      \"description\": \"The URIs that are used to indicate the namespaces of the SCIM schemas.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"urn:ietf:params:scim:schemas:core:2.0:Group\",\n          \"urn:ietf:params:scim:api:messages:2.0:ListResponse\"\n        ]\n      },\n      \"example\": [\n        \"urn:ietf:params:scim:schemas:core:2.0:Group\"\n      ]\n    },\n    \"externalId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the resource as defined by the provisioning client.\",\n      \"example\": \"8aa1a0c0-c4c3-4bc0-b4a5-2ef676900159\"\
  ,\n      \"nullable\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name for a security group.\",\n      \"example\": \"Engineering\",\n      \"nullable\": true\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"The group members.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"value\",\n          \"$ref\"\n        ],\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"The local unique identifier for the member\",\n            \"example\": \"23a35c27-23d3-4c03-b4c5-6443c09e7173\"\n          },\n          \"$ref\": {\n            \"type\": \"string\"\n          },\n          \"display\": {\n            \"type\": \"string\",\n            \"description\": \"The display name associated with the member\",\n            \"example\": \"Monalisa Octocat\"\n          }\n        }\n      }\n   \
  \ }\n  },\n  \"required\": [\n    \"schemas\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-scim-group-response-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: group-response
---
