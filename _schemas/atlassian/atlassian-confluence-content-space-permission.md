---
description: 'This object represents a permission for given space. Permissions consist of at least one operation object with an accompanying subjects object. The following combinations of `operation` and `targetType` values are valid for the `operation` object: - ''create'': ''page'', ''blogpost'', ''comment'', ''attachment'' - ''read'': ''space'' - ''delete'': ''page'', ''blogpost'', ''comment'', ''attachment'' - ''export'': ''space'' - ''administer'': ''space'''
layout: schema
name: SpacePermission
properties_list:
- description: ''
  name: id
  type: integer
- description: The users and/or groups that the permission applies to.
  name: subjects
  type: object
- description: Grant anonymous users permission to use the operation.
  name: anonymousAccess
  type: boolean
- description: Grants access to unlicensed users from JIRA Service Desk when used with the 'read space' operation.
  name: unlicensedAccess
  type: boolean
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-space-permission-schema.json
slug: atlassian-confluence-content-space-permission
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SpacePermission\",\n  \"type\": \"object\",\n  \"description\": \"This object represents a permission for given space. Permissions consist of\\nat least one operation object with an accompanying subjects object.\\n\\nThe following combinations of `operation` and `targetType` values are\\nvalid for the `operation` object:\\n\\n  - 'create': 'page', 'blogpost', 'comment', 'attachment'\\n  - 'read': 'space'\\n  - 'delete': 'page', 'blogpost', 'comment', 'attachment'\\n  - 'export': 'space'\\n  - 'administer': 'space'\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"subjects\": {\n      \"type\": \"object\",\n      \"description\": \"The users and/or groups that the permission applies to.\"\n    },\n    \"anonymousAccess\": {\n      \"type\": \"boolean\",\n      \"description\": \"Grant anonymous users permission to use the operation.\"\n    },\n    \"unlicensedAccess\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Grants access to unlicensed users from JIRA Service Desk when used\\nwith the 'read space' operation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-space-permission-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: SpacePermission
---
