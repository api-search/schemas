---
description: ListAccountPermissionsResponse schema
layout: schema
name: ListAccountPermissionsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: permissions
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-list-account-permissions-response-schema.json
slug: inspector-list-account-permissions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-account-permissions-response-schema.json\",\n  \"title\": \"ListAccountPermissionsResponse\",\n  \"description\": \"ListAccountPermissionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token to use for paginating results that are returned in the response. Set the value of this parameter to null for the first request to a list action. For subsequent calls, use the <code>NextToken</code> value returned from the previous request to continue listing results after the first page.\"\n        }\n      ]\n    },\n    \"permissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Permissions\"\
  \n        },\n        {\n          \"description\": \"Contains details on the permissions an account has to configure Amazon Inspector.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"permissions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-account-permissions-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ListAccountPermissionsResponse
---
