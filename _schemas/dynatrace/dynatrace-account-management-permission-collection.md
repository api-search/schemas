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
schema_file: json-schema/dynatrace-account-management-permission-collection-schema.json
slug: dynatrace-account-management-permission-collection
source_filename: dynatrace-account-management-permission-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A collection of permission assignments for the account.\",\n  \"properties\": {\n    \"permissions\": {\n      \"type\": \"array\",\n      \"description\": \"The list of all permissions in the account.\",\n      \"example\": [\n        {\n          \"permissionName\": \"Production Service\",\n          \"scope\": \"example-value\",\n          \"scopeType\": \"ACCOUNT\",\n          \"groupId\": \"abc123\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a permission assignment granting a group access to a Dynatrace environment or account-level capability.\",\n        \"properties\": {\n          \"permissionName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the permission, e.g., tenant-viewer, tenant-operator, tenant-admin, account-company-info.\",\n            \"example\": \"Production Service\"\n          },\n          \"scope\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"The scope identifier the permission applies to. For environment permissions, this is the environment ID. For account permissions, this is the account UUID.\",\n            \"example\": \"example-value\"\n          },\n          \"scopeType\": {\n            \"type\": \"string\",\n            \"description\": \"The type of scope. ACCOUNT for account-level permissions, TENANT for environment-level permissions.\",\n            \"example\": \"ACCOUNT\",\n            \"enum\": [\n              \"ACCOUNT\",\n              \"TENANT\"\n            ]\n          },\n          \"groupId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the group this permission is assigned to.\",\n            \"example\": \"abc123\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PermissionCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-account-management-permission-collection-schema.json
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
