---
description: DeregisterWorkspaceDirectoryRequest schema from Amazon WorkSpaces API
layout: schema
name: DeregisterWorkspaceDirectoryRequest
properties_list:
- description: ''
  name: DirectoryId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-deregister-workspace-directory-request-schema.json
slug: workspaces-deregister-workspace-directory-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"DirectoryId\"\n  ],\n  \"title\": \"DeregisterWorkspaceDirectoryRequest\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the directory. If any WorkSpaces are registered to this directory, you must remove them before you deregister the directory, or you will receive an OperationNotSupportedException error.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-deregister-workspace-directory-request-schema.json\",\n  \"description\": \"DeregisterWorkspaceDirectoryRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-deregister-workspace-directory-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DeregisterWorkspaceDirectoryRequest
---
