---
description: 'This object represents a single space permission. Permissions consist of at least one operation object with an accompanying subjects object. The following combinations of `operation.key` and `operation.target` values are valid for the `operation` object: ``` bash ''create'': ''page'', ''blogpost'', ''comment'', ''attachment'' ''read'': ''space'' ''delete'': ''page'', ''blogpost'', ''comment'', ''attachment'', ''space'' ''export'': ''space'' ''administer'': ''space'' ''archive'': ''page'' ''restrict_content'': ''space'' ``` For example, to enable Delete Own permission, set the `operation` object to the following: ``` "operation": { "key": "delete", "target": "space" } ``` To enable Add/Delete Restrictions permissions, set the `operation` object to the following: ``` "operation": { "key": "restrict_content", "target": "space" } ```'
layout: schema
name: SpacePermissionV2
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: operation
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-space-space-permission-v2-schema.json
slug: atlassian-confluence-space-space-permission-v2
source_filename: atlassian-confluence-space-space-permission-v2-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SpacePermissionV2\",\n  \"type\": \"object\",\n  \"description\": \"This object represents a single space permission. Permissions consist of\\nat least one operation object with an accompanying subjects object.\\n\\nThe following combinations of `operation.key` and `operation.target` values are\\nvalid for the `operation` object:\\n``` bash\\n'create': 'page', 'blogpost', 'comment', 'attachment'\\n'read': 'space'\\n'delete': 'page', 'blogpost', 'comment', 'attachment', 'space'\\n'export': 'space'\\n'administer': 'space'\\n'archive': 'page'\\n'restrict_content': 'space'\\n```\\n\\nFor example, to enable Delete Own permission, set the `operation` object to the following:\\n```\\n\\\"operation\\\": {\\n    \\\"key\\\": \\\"delete\\\",\\n    \\\"target\\\": \\\"space\\\"\\n}\\n```\\nTo enable Add/Delete Restrictions permissions, set the `operation` object to the following:\\n```\\n\\\"operation\\\
  \": {\\n    \\\"key\\\": \\\"restrict_content\\\",\\n    \\\"target\\\": \\\"space\\\"\\n}\\n```\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"operation\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-space-space-permission-v2-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: SpacePermissionV2
---
