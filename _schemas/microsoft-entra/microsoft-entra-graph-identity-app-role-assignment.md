---
description: Represents an app role granted to a user, group, or service principal
layout: schema
name: AppRoleAssignment
properties_list:
- description: Unique identifier for the assignment (GUID)
  name: id
  type: string
- description: The ID of the app role to assign. Use the default role ID 00000000-0000-0000-0000-000000000000 for default access.
  name: appRoleId
  type: string
- description: The unique identifier of the user, group, or service principal being granted the app role
  name: principalId
  type: string
- description: The type of the assigned principal
  name: principalType
  type: string
- description: Display name of the principal
  name: principalDisplayName
  type: string
- description: The unique identifier of the resource service principal to which the assignment is made
  name: resourceId
  type: string
- description: Display name of the resource application
  name: resourceDisplayName
  type: string
- description: Time when the app role assignment was created
  name: createdDateTime
  type: string
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-app-role-assignment-schema.json
slug: microsoft-entra-graph-identity-app-role-assignment
source_filename: microsoft-entra-graph-identity-app-role-assignment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AppRoleAssignment\",\n  \"type\": \"object\",\n  \"description\": \"Represents an app role granted to a user, group, or service principal\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the assignment (GUID)\"\n    },\n    \"appRoleId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the app role to assign. Use the default role ID 00000000-0000-0000-0000-000000000000 for default access.\"\n    },\n    \"principalId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the user, group, or service principal being granted the app role\"\n    },\n    \"principalType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the assigned principal\"\n    },\n    \"principalDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the principal\"\
  \n    },\n    \"resourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the resource service principal to which the assignment is made\"\n    },\n    \"resourceDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the resource application\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time when the app role assignment was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-app-role-assignment-schema.json
tags:
- Access Management
- Authentication
- Azure AD
- Entra
- Identity
- Identity Governance
- Microsoft
- Network Security
- Security
- Zero Trust
title: AppRoleAssignment
---
