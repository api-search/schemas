---
description: DescribeIpGroupsRequest schema from Amazon WorkSpaces API
layout: schema
name: DescribeIpGroupsRequest
properties_list:
- description: ''
  name: GroupIds
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-ip-groups-request-schema.json
slug: workspaces-describe-ip-groups-request
source_filename: workspaces-describe-ip-groups-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"DescribeIpGroupsRequest\",\n  \"properties\": {\n    \"GroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupIdList\"\n        },\n        {\n          \"description\": \"The identifiers of one or more IP access control groups.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If you received a <code>NextToken</code> from a previous call that was paginated, provide this token to receive the next set of results.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of items to return.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\"\
  : \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-ip-groups-request-schema.json\",\n  \"description\": \"DescribeIpGroupsRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-ip-groups-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeIpGroupsRequest
---
