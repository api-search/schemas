---
description: DescribeWorkspaceBundlesResult schema from Amazon WorkSpaces API
layout: schema
name: DescribeWorkspaceBundlesResult
properties_list:
- description: ''
  name: Bundles
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-workspace-bundles-result-schema.json
slug: workspaces-describe-workspace-bundles-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bundles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BundleList\"\n        },\n        {\n          \"description\": \"Information about the bundles.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. This value is null when there are no more results to return. This token is valid for one day and must be used within that time frame.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeWorkspaceBundlesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-bundles-result-schema.json\",\n  \"description\": \"DescribeWorkspaceBundlesResult\
  \ schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-workspace-bundles-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeWorkspaceBundlesResult
---
