---
description: DescribeWorkspacesResult schema from Amazon WorkSpaces API
layout: schema
name: DescribeWorkspacesResult
properties_list:
- description: ''
  name: Workspaces
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-workspaces-result-schema.json
slug: workspaces-describe-workspaces-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Workspaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceList\"\n        },\n        {\n          \"description\": \"<p>Information about the WorkSpaces.</p> <p>Because <a>CreateWorkspaces</a> is an asynchronous operation, some of the returned information could be incomplete.</p>\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. This value is null when there are no more results to return. \"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeWorkspacesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspaces-result-schema.json\"\
  ,\n  \"description\": \"DescribeWorkspacesResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspaces-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeWorkspacesResult
---
