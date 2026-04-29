---
description: Information about the standby WorkSpace.
layout: schema
name: PendingCreateStandbyWorkspacesRequest
properties_list:
- description: ''
  name: UserName
  type: object
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: WorkspaceId
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-pending-create-standby-workspaces-request-schema.json
slug: workspaces-pending-create-standby-workspaces-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"<p>Describes the standby WorkSpace that was created.</p> <p>Because this operation is asynchronous, the identifier returned is not immediately available for use with other operations. For example, if you call <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/api/API_DescribeWorkspaces.html\\\"> DescribeWorkspaces</a> before the WorkSpace is created, the information returned can be incomplete. </p>\"\n        }\n      ]\n    },\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the directory for the standby WorkSpace.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceState\"\
  \n        },\n        {\n          \"description\": \"The operational state of the standby WorkSpace.\"\n        }\n      ]\n    },\n    \"WorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The identifier of the standby WorkSpace.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about the standby WorkSpace.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PendingCreateStandbyWorkspacesRequest\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-pending-create-standby-workspaces-request-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-pending-create-standby-workspaces-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: PendingCreateStandbyWorkspacesRequest
---
