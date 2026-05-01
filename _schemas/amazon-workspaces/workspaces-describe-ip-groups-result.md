---
description: DescribeIpGroupsResult schema from Amazon WorkSpaces API
layout: schema
name: DescribeIpGroupsResult
properties_list:
- description: ''
  name: Result
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-ip-groups-result-schema.json
slug: workspaces-describe-ip-groups-result
source_filename: workspaces-describe-ip-groups-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspacesIpGroupsList\"\n        },\n        {\n          \"description\": \"Information about the IP access control groups.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. This value is null when there are no more results to return. \"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeIpGroupsResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-ip-groups-result-schema.json\",\n  \"description\": \"DescribeIpGroupsResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-ip-groups-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeIpGroupsResult
---
