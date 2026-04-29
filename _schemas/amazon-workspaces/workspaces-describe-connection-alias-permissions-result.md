---
description: DescribeConnectionAliasPermissionsResult schema from Amazon WorkSpaces API
layout: schema
name: DescribeConnectionAliasPermissionsResult
properties_list:
- description: ''
  name: AliasId
  type: object
- description: ''
  name: ConnectionAliasPermissions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-connection-alias-permissions-result-schema.json
slug: workspaces-describe-connection-alias-permissions-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasId\"\n        },\n        {\n          \"description\": \"The identifier of the connection alias.\"\n        }\n      ]\n    },\n    \"ConnectionAliasPermissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionAliasPermissions\"\n        },\n        {\n          \"description\": \"The permissions associated with a connection alias.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The token to use to retrieve the next page of results. This value is null when there are no more results to return. \"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeConnectionAliasPermissionsResult\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-connection-alias-permissions-result-schema.json\",\n  \"description\": \"DescribeConnectionAliasPermissionsResult schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-connection-alias-permissions-result-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeConnectionAliasPermissionsResult
---
