---
description: ListAvailableManagementCidrRangesResult schema from Amazon WorkSpaces API
layout: schema
name: ListAvailableManagementCidrRangesResult
properties_list:
- description: ''
  name: ManagementCidrRanges
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-list-available-management-cidr-ranges-result-schema.json
slug: workspaces-list-available-management-cidr-ranges-result
source_filename: workspaces-list-available-management-cidr-ranges-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ManagementCidrRanges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DedicatedTenancyCidrRangeList\"\n        },\n        {\n          \"description\": \"The list of available IP address ranges, specified as IPv4 CIDR blocks.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. This value is null when there are no more results to return. \"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListAvailableManagementCidrRangesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-list-available-management-cidr-ranges-result-schema.json\",\n  \"description\":\
  \ \"ListAvailableManagementCidrRangesResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-list-available-management-cidr-ranges-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ListAvailableManagementCidrRangesResult
---
