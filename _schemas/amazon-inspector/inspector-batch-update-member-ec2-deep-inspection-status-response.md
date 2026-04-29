---
description: BatchUpdateMemberEc2DeepInspectionStatusResponse schema
layout: schema
name: BatchUpdateMemberEc2DeepInspectionStatusResponse
properties_list:
- description: ''
  name: accountIds
  type: object
- description: ''
  name: failedAccountIds
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-update-member-ec2-deep-inspection-status-response-schema.json
slug: inspector-batch-update-member-ec2-deep-inspection-status-response
source_filename: inspector-batch-update-member-ec2-deep-inspection-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-update-member-ec2-deep-inspection-status-response-schema.json\",\n  \"title\": \"BatchUpdateMemberEc2DeepInspectionStatusResponse\",\n  \"description\": \"BatchUpdateMemberEc2DeepInspectionStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberAccountEc2DeepInspectionStatusStateList\"\n        },\n        {\n          \"description\": \"An array of objects that provide details for each of the accounts that Amazon Inspector deep inspection status was successfully changed for. \"\n        }\n      ]\n    },\n    \"failedAccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedMemberAccountEc2DeepInspectionStatusStateList\"\n     \
  \   },\n        {\n          \"description\": \"An array of objects that provide details for each of the accounts that Amazon Inspector deep inspection status could not be successfully changed for. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-update-member-ec2-deep-inspection-status-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchUpdateMemberEc2DeepInspectionStatusResponse
---
