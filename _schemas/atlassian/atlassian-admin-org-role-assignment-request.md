---
description: Request body for assigning or revoking organization-level roles.
layout: schema
name: OrgRoleAssignmentRequest
properties_list:
- description: The organization-level role to assign or revoke. Common roles include org-admin, trusted-user, and user.
  name: role
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-org-role-assignment-request-schema.json
slug: atlassian-admin-org-role-assignment-request
source_filename: atlassian-admin-org-role-assignment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrgRoleAssignmentRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for assigning or revoking organization-level roles.\",\n  \"properties\": {\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The organization-level role to assign or revoke. Common roles include org-admin, trusted-user, and user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-org-role-assignment-request-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: OrgRoleAssignmentRequest
---
