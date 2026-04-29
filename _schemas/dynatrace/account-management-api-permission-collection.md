---
description: A collection of permission assignments for the account.
layout: schema
name: PermissionCollection
properties_list:
- description: The list of all permissions in the account.
  name: permissions
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/account-management-api-permission-collection-schema.json
slug: account-management-api-permission-collection
source_filename: account-management-api-permission-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-permission-collection-schema.json\",\n  \"title\": \"PermissionCollection\",\n  \"description\": \"A collection of permission assignments for the account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permissions\": {\n      \"type\": \"array\",\n      \"description\": \"The list of all permissions in the account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Permission\"\n      },\n      \"example\": [\n        {\n          \"permissionName\": \"Production Service\",\n          \"scope\": \"example-value\",\n          \"scopeType\": \"ACCOUNT\",\n          \"groupId\": \"abc123\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/account-management-api-permission-collection-schema.json
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
title: PermissionCollection
---
