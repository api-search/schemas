---
description: DescribeWorkspacesConnectionStatusRequest schema from Amazon WorkSpaces API
layout: schema
name: DescribeWorkspacesConnectionStatusRequest
properties_list:
- description: ''
  name: WorkspaceIds
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-workspaces-connection-status-request-schema.json
slug: workspaces-describe-workspaces-connection-status-request
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"DescribeWorkspacesConnectionStatusRequest\",\n  \"properties\": {\n    \"WorkspaceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceIdList\"\n        },\n        {\n          \"description\": \"The identifiers of the WorkSpaces. You can specify up to 25 WorkSpaces.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If you received a <code>NextToken</code> from a previous call that was paginated, provide this token to receive the next set of results.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspaces-connection-status-request-schema.json\",\n  \"description\"\
  : \"DescribeWorkspacesConnectionStatusRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspaces-connection-status-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeWorkspacesConnectionStatusRequest
---
