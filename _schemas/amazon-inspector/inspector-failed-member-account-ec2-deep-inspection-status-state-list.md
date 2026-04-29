---
description: FailedMemberAccountEc2DeepInspectionStatusStateList schema
layout: schema
name: FailedMemberAccountEc2DeepInspectionStatusStateList
properties_list: []
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-failed-member-account-ec2-deep-inspection-status-state-list-schema.json
slug: inspector-failed-member-account-ec2-deep-inspection-status-state-list
source_filename: inspector-failed-member-account-ec2-deep-inspection-status-state-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-failed-member-account-ec2-deep-inspection-status-state-list-schema.json\",\n  \"title\": \"FailedMemberAccountEc2DeepInspectionStatusStateList\",\n  \"description\": \"FailedMemberAccountEc2DeepInspectionStatusStateList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"accountId\"\n    ],\n    \"properties\": {\n      \"accountId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AccountId\"\n          },\n          {\n            \"description\": \"The unique identifier for the Amazon Web Services account of the organization member that failed to activate Amazon Inspector deep inspection.\"\n          }\n        ]\n      },\n      \"ec2ScanStatus\": {\n        \"allOf\": [\n          {\n            \"\
  $ref\": \"#/components/schemas/Status\"\n          },\n          {\n            \"description\": \"The status of EC2 scanning in the account that failed to activate Amazon Inspector deep inspection.\"\n          }\n        ]\n      },\n      \"errorMessage\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The error message explaining why the account failed to activate Amazon Inspector deep inspection.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that contains details about a member account in your organization that failed to activate Amazon Inspector deep inspection.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-failed-member-account-ec2-deep-inspection-status-state-list-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: FailedMemberAccountEc2DeepInspectionStatusStateList
---
