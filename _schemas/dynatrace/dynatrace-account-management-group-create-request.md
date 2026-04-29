---
description: Request body for creating or updating a group.
layout: schema
name: GroupCreateRequest
properties_list:
- description: The display name of the group.
  name: name
  type: string
- description: An optional description of the group's purpose or access scope.
  name: description
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-account-management-group-create-request-schema.json
slug: dynatrace-account-management-group-create-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Request body for creating or updating a group.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the group.\",\n      \"example\": \"Production Service\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"An optional description of the group's purpose or access scope.\",\n      \"example\": \"Example description.\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupCreateRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-account-management-group-create-request-schema.json
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
title: GroupCreateRequest
---
