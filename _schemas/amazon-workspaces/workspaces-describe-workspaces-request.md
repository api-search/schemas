---
description: DescribeWorkspacesRequest schema from Amazon WorkSpaces API
layout: schema
name: DescribeWorkspacesRequest
properties_list:
- description: ''
  name: WorkspaceIds
  type: object
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: UserName
  type: object
- description: ''
  name: BundleId
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-workspaces-request-schema.json
slug: workspaces-describe-workspaces-request
source_filename: workspaces-describe-workspaces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"DescribeWorkspacesRequest\",\n  \"properties\": {\n    \"WorkspaceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceIdList\"\n        },\n        {\n          \"description\": \"<p>The identifiers of the WorkSpaces. You cannot combine this parameter with any other filter.</p> <p>Because the <a>CreateWorkspaces</a> operation is asynchronous, the identifier it returns is not immediately available. If you immediately call <a>DescribeWorkspaces</a> with this identifier, no information is returned.</p>\"\n        }\n      ]\n    },\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the directory. In addition, you can optionally specify a specific directory user (see <code>UserName</code>). You cannot combine this parameter with any other filter.\"\n        }\n   \
  \   ]\n    },\n    \"UserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"The name of the directory user. You must specify this parameter with <code>DirectoryId</code>.\"\n        }\n      ]\n    },\n    \"BundleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleId\"\n        },\n        {\n          \"description\": \"The identifier of the bundle. All WorkSpaces that are created from this bundle are retrieved. You cannot combine this parameter with any other filter.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of items to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n\
  \          \"description\": \"If you received a <code>NextToken</code> from a previous call that was paginated, provide this token to receive the next set of results.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspaces-request-schema.json\",\n  \"description\": \"DescribeWorkspacesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspaces-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeWorkspacesRequest
---
