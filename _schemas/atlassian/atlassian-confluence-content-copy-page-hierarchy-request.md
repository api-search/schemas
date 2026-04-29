---
description: ''
layout: schema
name: CopyPageHierarchyRequest
properties_list:
- description: If set to `true`, attachments are copied to the destination page.
  name: copyAttachments
  type: boolean
- description: If set to `true`, page permissions are copied to the destination page.
  name: copyPermissions
  type: boolean
- description: If set to `true`, content properties are copied to the destination page.
  name: copyProperties
  type: boolean
- description: If set to `true`, labels are copied to the destination page.
  name: copyLabels
  type: boolean
- description: If set to `true`, custom contents are copied to the destination page.
  name: copyCustomContents
  type: boolean
- description: If set to `true`, descendants are copied to the destination page.
  name: copyDescendants
  type: boolean
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-copy-page-hierarchy-request-schema.json
slug: atlassian-confluence-content-copy-page-hierarchy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopyPageHierarchyRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"copyAttachments\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to `true`, attachments are copied to the destination page.\"\n    },\n    \"copyPermissions\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to `true`, page permissions are copied to the destination page.\"\n    },\n    \"copyProperties\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to `true`, content properties are copied to the destination page.\"\n    },\n    \"copyLabels\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to `true`, labels are copied to the destination page.\"\n    },\n    \"copyCustomContents\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to `true`, custom contents are copied to the destination page.\"\n    },\n    \"copyDescendants\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"If set to `true`, descendants are copied to the destination page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-copy-page-hierarchy-request-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: CopyPageHierarchyRequest
---
