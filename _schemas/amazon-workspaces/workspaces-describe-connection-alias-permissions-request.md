---
description: DescribeConnectionAliasPermissionsRequest schema from Amazon WorkSpaces API
layout: schema
name: DescribeConnectionAliasPermissionsRequest
properties_list:
- description: ''
  name: AliasId
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-connection-alias-permissions-request-schema.json
slug: workspaces-describe-connection-alias-permissions-request
source_filename: workspaces-describe-connection-alias-permissions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"AliasId\"\n  ],\n  \"title\": \"DescribeConnectionAliasPermissionsRequest\",\n  \"properties\": {\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasId\"\n        },\n        {\n          \"description\": \"The identifier of the connection alias.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If you received a <code>NextToken</code> from a previous call that was paginated, provide this token to receive the next set of results. \"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of results to return.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-connection-alias-permissions-request-schema.json\",\n  \"description\": \"DescribeConnectionAliasPermissionsRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-connection-alias-permissions-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeConnectionAliasPermissionsRequest
---
