---
description: CreateWorkspacesResult schema from Amazon WorkSpaces API
layout: schema
name: CreateWorkspacesResult
properties_list:
- description: ''
  name: FailedRequests
  type: object
- description: ''
  name: PendingRequests
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-create-workspaces-result-schema.json
slug: workspaces-create-workspaces-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailedRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedCreateWorkspaceRequests\"\n        },\n        {\n          \"description\": \"Information about the WorkSpaces that could not be created.\"\n        }\n      ]\n    },\n    \"PendingRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceList\"\n        },\n        {\n          \"description\": \"<p>Information about the WorkSpaces that were created.</p> <p>Because this operation is asynchronous, the identifier returned is not immediately available for use with other operations. For example, if you call <a>DescribeWorkspaces</a> before the WorkSpace is created, the information returned can be incomplete.</p>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateWorkspacesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-workspaces-result-schema.json\"\
  ,\n  \"description\": \"CreateWorkspacesResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-create-workspaces-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CreateWorkspacesResult
---
