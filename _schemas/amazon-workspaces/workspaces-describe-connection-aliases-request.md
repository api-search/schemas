---
description: DescribeConnectionAliasesRequest schema from Amazon WorkSpaces API
layout: schema
name: DescribeConnectionAliasesRequest
properties_list:
- description: ''
  name: AliasIds
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-connection-aliases-request-schema.json
slug: workspaces-describe-connection-aliases-request
source_filename: workspaces-describe-connection-aliases-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"DescribeConnectionAliasesRequest\",\n  \"properties\": {\n    \"AliasIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasIdList\"\n        },\n        {\n          \"description\": \"The identifiers of the connection aliases to describe.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The identifier of the directory associated with the connection alias.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of connection aliases to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n\
  \        {\n          \"description\": \"If you received a <code>NextToken</code> from a previous call that was paginated, provide this token to receive the next set of results. \"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-connection-aliases-request-schema.json\",\n  \"description\": \"DescribeConnectionAliasesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-connection-aliases-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeConnectionAliasesRequest
---
