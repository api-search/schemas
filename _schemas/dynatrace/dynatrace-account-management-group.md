---
description: Represents a user group in the Dynatrace account.
layout: schema
name: Group
properties_list:
- description: The unique identifier of the group.
  name: groupId
  type: string
- description: The display name of the group.
  name: name
  type: string
- description: An optional description of the group's purpose or scope.
  name: description
  type: string
- description: The identifier of the group owner. LOCAL indicates the group is managed within Dynatrace; SSO indicates it is synced from an identity provider.
  name: owner
  type: string
- description: The date and time when the group was created.
  name: createdAt
  type: string
- description: The date and time when the group was last updated.
  name: updatedAt
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-account-management-group-schema.json
slug: dynatrace-account-management-group
source_filename: dynatrace-account-management-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents a user group in the Dynatrace account.\",\n  \"properties\": {\n    \"groupId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the group.\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the group.\",\n      \"example\": \"Production Service\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"An optional description of the group's purpose or scope.\",\n      \"example\": \"Example description.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the group owner. LOCAL indicates the group is managed within Dynatrace; SSO indicates it is synced from an identity provider.\",\n      \"example\": \"example-value\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when\
  \ the group was created.\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the group was last updated.\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Group\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-account-management-group-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: Group
---
