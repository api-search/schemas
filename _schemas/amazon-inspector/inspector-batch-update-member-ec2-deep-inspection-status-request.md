---
description: BatchUpdateMemberEc2DeepInspectionStatusRequest schema
layout: schema
name: BatchUpdateMemberEc2DeepInspectionStatusRequest
properties_list:
- description: ''
  name: accountIds
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-update-member-ec2-deep-inspection-status-request-schema.json
slug: inspector-batch-update-member-ec2-deep-inspection-status-request
source_filename: inspector-batch-update-member-ec2-deep-inspection-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-update-member-ec2-deep-inspection-status-request-schema.json\",\n  \"title\": \"BatchUpdateMemberEc2DeepInspectionStatusRequest\",\n  \"description\": \"BatchUpdateMemberEc2DeepInspectionStatusRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberAccountEc2DeepInspectionStatusList\"\n        },\n        {\n          \"description\": \"The unique identifiers for the Amazon Web Services accounts to change Amazon Inspector deep inspection status for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-update-member-ec2-deep-inspection-status-request-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchUpdateMemberEc2DeepInspectionStatusRequest
---
