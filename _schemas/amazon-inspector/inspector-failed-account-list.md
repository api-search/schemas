---
description: FailedAccountList schema
layout: schema
name: FailedAccountList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-failed-account-list-schema.json
slug: inspector-failed-account-list
source_filename: inspector-failed-account-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-failed-account-list-schema.json\",\n  \"title\": \"FailedAccountList\",\n  \"description\": \"FailedAccountList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"accountId\",\n      \"errorCode\",\n      \"errorMessage\"\n    ],\n    \"properties\": {\n      \"accountId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AccountId\"\n          },\n          {\n            \"description\": \"The Amazon Web Services account ID.\"\n          }\n        ]\n      },\n      \"errorCode\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ErrorCode\"\n          },\n          {\n            \"description\": \"The error code explaining why the account failed to enable Amazon Inspector.\"\
  \n          }\n        ]\n      },\n      \"errorMessage\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The error message received when the account failed to enable Amazon Inspector.\"\n          }\n        ]\n      },\n      \"resourceStatus\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceStatus\"\n          },\n          {\n            \"description\": \"An object detailing which resources Amazon Inspector is enabled to scan for the account.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Status\"\n          },\n          {\n            \"description\": \"The status of Amazon Inspector for the account.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object with details on why an account failed to enable Amazon Inspector.\"\
  \n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-failed-account-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: FailedAccountList
---
