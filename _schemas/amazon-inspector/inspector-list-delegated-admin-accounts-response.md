---
description: ListDelegatedAdminAccountsResponse schema
layout: schema
name: ListDelegatedAdminAccountsResponse
properties_list:
- description: ''
  name: delegatedAdminAccounts
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-list-delegated-admin-accounts-response-schema.json
slug: inspector-list-delegated-admin-accounts-response
source_filename: inspector-list-delegated-admin-accounts-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-delegated-admin-accounts-response-schema.json\",\n  \"title\": \"ListDelegatedAdminAccountsResponse\",\n  \"description\": \"ListDelegatedAdminAccountsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"delegatedAdminAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DelegatedAdminAccountList\"\n        },\n        {\n          \"description\": \"Details of the Amazon Inspector delegated administrator of your organization.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token to use for paginating results that are returned in the response. Set the value of this parameter to null for the\
  \ first request to a list action. For subsequent calls, use the <code>NextToken</code> value returned from the previous request to continue listing results after the first page.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-list-delegated-admin-accounts-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: ListDelegatedAdminAccountsResponse
---
