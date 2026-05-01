---
description: DescribeConnectionAliasesResult schema from Amazon WorkSpaces API
layout: schema
name: DescribeConnectionAliasesResult
properties_list:
- description: ''
  name: ConnectionAliases
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-connection-aliases-result-schema.json
slug: workspaces-describe-connection-aliases-result
source_filename: workspaces-describe-connection-aliases-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionAliases\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasList\"\n        },\n        {\n          \"description\": \"Information about the specified connection aliases.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. This value is null when there are no more results to return. \"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeConnectionAliasesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-connection-aliases-result-schema.json\",\n  \"description\": \"DescribeConnectionAliasesResult schema from Amazon\
  \ WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-connection-aliases-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeConnectionAliasesResult
---
