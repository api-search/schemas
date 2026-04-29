---
description: DescribeWorkspaceDirectoriesRequest schema from Amazon WorkSpaces API
layout: schema
name: DescribeWorkspaceDirectoriesRequest
properties_list:
- description: ''
  name: DirectoryIds
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-workspace-directories-request-schema.json
slug: workspaces-describe-workspace-directories-request
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"DescribeWorkspaceDirectoriesRequest\",\n  \"properties\": {\n    \"DirectoryIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryIdList\"\n        },\n        {\n          \"description\": \"The identifiers of the directories. If the value is null, all directories are retrieved.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of directories to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If you received a <code>NextToken</code> from a previous call that was paginated, provide this token to receive the next set of results.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-directories-request-schema.json\",\n  \"description\": \"DescribeWorkspaceDirectoriesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-directories-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeWorkspaceDirectoriesRequest
---
