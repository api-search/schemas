---
description: 'This object represents the response for the content permission check API. If the user or group does not have permissions, the following errors may be returned: - Group does not have permission to the space - Group does not have permission to the content - User is not allowed to use Confluence - User does not have permission to the space - User does not have permission to the content - Anonymous users are not allowed to use Confluence - Anonymous user does not have permission to the space - Anonymous user does not have permission to the content'
layout: schema
name: PermissionCheckResponse
properties_list:
- description: ''
  name: hasPermission
  type: boolean
- description: ''
  name: errors
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-permission-check-response-schema.json
slug: atlassian-confluence-content-permission-check-response
source_filename: atlassian-confluence-content-permission-check-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PermissionCheckResponse\",\n  \"type\": \"object\",\n  \"description\": \"This object represents the response for the content permission check API. If the user or group does not have\\npermissions, the following errors may be returned:\\n\\n- Group does not have permission to the space\\n- Group does not have permission to the content\\n- User is not allowed to use Confluence\\n- User does not have permission to the space\\n- User does not have permission to the content\\n- Anonymous users are not allowed to use Confluence\\n- Anonymous user does not have permission to the space\\n- Anonymous user does not have permission to the content\",\n  \"properties\": {\n    \"hasPermission\": {\n      \"type\": \"boolean\"\n    },\n    \"errors\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-permission-check-response-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: PermissionCheckResponse
---
