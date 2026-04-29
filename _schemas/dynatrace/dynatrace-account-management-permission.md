---
description: Represents a permission assignment granting a group access to a Dynatrace environment or account-level capability.
layout: schema
name: Permission
properties_list:
- description: The name of the permission, e.g., tenant-viewer, tenant-operator, tenant-admin, account-company-info.
  name: permissionName
  type: string
- description: The scope identifier the permission applies to. For environment permissions, this is the environment ID. For account permissions, this is the account UUID.
  name: scope
  type: string
- description: The type of scope. ACCOUNT for account-level permissions, TENANT for environment-level permissions.
  name: scopeType
  type: string
- description: The ID of the group this permission is assigned to.
  name: groupId
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-account-management-permission-schema.json
slug: dynatrace-account-management-permission
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents a permission assignment granting a group access to a Dynatrace environment or account-level capability.\",\n  \"properties\": {\n    \"permissionName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the permission, e.g., tenant-viewer, tenant-operator, tenant-admin, account-company-info.\",\n      \"example\": \"Production Service\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"The scope identifier the permission applies to. For environment permissions, this is the environment ID. For account permissions, this is the account UUID.\",\n      \"example\": \"example-value\"\n    },\n    \"scopeType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of scope. ACCOUNT for account-level permissions, TENANT for environment-level permissions.\",\n      \"example\": \"ACCOUNT\",\n      \"enum\": [\n        \"ACCOUNT\",\n        \"TENANT\"\n      ]\n\
  \    },\n    \"groupId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the group this permission is assigned to.\",\n      \"example\": \"abc123\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Permission\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-account-management-permission-schema.json
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
title: Permission
---
