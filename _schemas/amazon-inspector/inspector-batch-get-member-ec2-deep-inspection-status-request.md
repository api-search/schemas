---
description: BatchGetMemberEc2DeepInspectionStatusRequest schema
layout: schema
name: BatchGetMemberEc2DeepInspectionStatusRequest
properties_list:
- description: ''
  name: accountIds
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-get-member-ec2-deep-inspection-status-request-schema.json
slug: inspector-batch-get-member-ec2-deep-inspection-status-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-member-ec2-deep-inspection-status-request-schema.json\",\n  \"title\": \"BatchGetMemberEc2DeepInspectionStatusRequest\",\n  \"description\": \"BatchGetMemberEc2DeepInspectionStatusRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIdSet\"\n        },\n        {\n          \"description\": \"The unique identifiers for the Amazon Web Services accounts to retrieve Amazon Inspector deep inspection activation status for. <pre><code> &lt;/p&gt; </code></pre>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-member-ec2-deep-inspection-status-request-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchGetMemberEc2DeepInspectionStatusRequest
---
