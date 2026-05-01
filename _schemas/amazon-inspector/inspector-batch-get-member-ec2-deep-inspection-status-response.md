---
description: BatchGetMemberEc2DeepInspectionStatusResponse schema
layout: schema
name: BatchGetMemberEc2DeepInspectionStatusResponse
properties_list:
- description: ''
  name: accountIds
  type: object
- description: ''
  name: failedAccountIds
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-get-member-ec2-deep-inspection-status-response-schema.json
slug: inspector-batch-get-member-ec2-deep-inspection-status-response
source_filename: inspector-batch-get-member-ec2-deep-inspection-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-member-ec2-deep-inspection-status-response-schema.json\",\n  \"title\": \"BatchGetMemberEc2DeepInspectionStatusResponse\",\n  \"description\": \"BatchGetMemberEc2DeepInspectionStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberAccountEc2DeepInspectionStatusStateList\"\n        },\n        {\n          \"description\": \"An array of objects that provide details on the activation status of Amazon Inspector deep inspection for each of the requested accounts. <pre><code> &lt;/p&gt; </code></pre>\"\n        }\n      ]\n    },\n    \"failedAccountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedMemberAccountEc2DeepInspectionStatusStateList\"\
  \n        },\n        {\n          \"description\": \"An array of objects that provide details on any accounts that failed to activate Amazon Inspector deep inspection and why. <pre><code> &lt;/p&gt; </code></pre>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-member-ec2-deep-inspection-status-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchGetMemberEc2DeepInspectionStatusResponse
---
