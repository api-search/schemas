---
description: ListAvailableManagementCidrRangesRequest schema from Amazon WorkSpaces API
layout: schema
name: ListAvailableManagementCidrRangesRequest
properties_list:
- description: ''
  name: ManagementCidrRangeConstraint
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-list-available-management-cidr-ranges-request-schema.json
slug: workspaces-list-available-management-cidr-ranges-request
source_filename: workspaces-list-available-management-cidr-ranges-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ManagementCidrRangeConstraint\"\n  ],\n  \"title\": \"ListAvailableManagementCidrRangesRequest\",\n  \"properties\": {\n    \"ManagementCidrRangeConstraint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManagementCidrRangeConstraint\"\n        },\n        {\n          \"description\": \"The IP address range to search. Specify an IP address range that is compatible with your network and in CIDR notation (that is, specify the range as an IPv4 CIDR block).\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManagementCidrRangeMaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of items to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\"\
  : \"If you received a <code>NextToken</code> from a previous call that was paginated, provide this token to receive the next set of results.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-list-available-management-cidr-ranges-request-schema.json\",\n  \"description\": \"ListAvailableManagementCidrRangesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-list-available-management-cidr-ranges-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ListAvailableManagementCidrRangesRequest
---
