---
description: DisableDelegatedAdminAccountRequest schema
layout: schema
name: DisableDelegatedAdminAccountRequest
properties_list:
- description: ''
  name: delegatedAdminAccountId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-disable-delegated-admin-account-request-schema.json
slug: inspector-disable-delegated-admin-account-request
source_filename: inspector-disable-delegated-admin-account-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-disable-delegated-admin-account-request-schema.json\",\n  \"title\": \"DisableDelegatedAdminAccountRequest\",\n  \"description\": \"DisableDelegatedAdminAccountRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"delegatedAdminAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the current Amazon Inspector delegated administrator.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"delegatedAdminAccountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-disable-delegated-admin-account-request-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: DisableDelegatedAdminAccountRequest
---
