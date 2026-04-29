---
description: An object that contains details about the status of Amazon Inspector deep inspection for a member account in your organization.
layout: schema
name: MemberAccountEc2DeepInspectionStatus
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: activateDeepInspection
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-member-account-ec2-deep-inspection-status-schema.json
slug: inspector-member-account-ec2-deep-inspection-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-member-account-ec2-deep-inspection-status-schema.json\",\n  \"title\": \"MemberAccountEc2DeepInspectionStatus\",\n  \"description\": \"An object that contains details about the status of Amazon Inspector deep inspection for a member account in your organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The unique identifier for the Amazon Web Services account of the organization member.\"\n        }\n      ]\n    },\n    \"activateDeepInspection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether Amazon Inspector deep inspection\
  \ is active in the account. If <code>TRUE</code> Amazon Inspector deep inspection is active, if <code>FALSE</code> it is not active.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountId\",\n    \"activateDeepInspection\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-member-account-ec2-deep-inspection-status-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: MemberAccountEc2DeepInspectionStatus
---
