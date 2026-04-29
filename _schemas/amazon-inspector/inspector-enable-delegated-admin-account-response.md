---
description: EnableDelegatedAdminAccountResponse schema
layout: schema
name: EnableDelegatedAdminAccountResponse
properties_list:
- description: ''
  name: delegatedAdminAccountId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-enable-delegated-admin-account-response-schema.json
slug: inspector-enable-delegated-admin-account-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-enable-delegated-admin-account-response-schema.json\",\n  \"title\": \"EnableDelegatedAdminAccountResponse\",\n  \"description\": \"EnableDelegatedAdminAccountResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"delegatedAdminAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the successfully Amazon Inspector delegated administrator.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"delegatedAdminAccountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-enable-delegated-admin-account-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: EnableDelegatedAdminAccountResponse
---
