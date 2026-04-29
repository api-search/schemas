---
description: High-level information about the managed rule group that your own rule group is copied from. You can use the the metadata to track version updates made to the originating rule group. You can retrieve all objects for a rule group by calling <a href="https://docs.aws.amazon.com/network-firewall/latest/APIReference/API_DescribeRuleGroup.html">DescribeRuleGroup</a>.
layout: schema
name: SourceMetadata
properties_list:
- description: ''
  name: SourceArn
  type: object
- description: ''
  name: SourceUpdateToken
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-source-metadata-schema.json
slug: openapi-source-metadata
source_filename: openapi-source-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-source-metadata-schema.json\",\n  \"title\": \"SourceMetadata\",\n  \"description\": \"High-level information about the managed rule group that your own rule group is copied from. You can use the the metadata to track version updates made to the originating rule group. You can retrieve all objects for a rule group by calling <a href=\\\"https://docs.aws.amazon.com/network-firewall/latest/APIReference/API_DescribeRuleGroup.html\\\">DescribeRuleGroup</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the rule group that your own rule group is copied from.\"\n        }\n      ]\n    },\n    \"\
  SourceUpdateToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateToken\"\n        },\n        {\n          \"description\": \"The update token of the Amazon Web Services managed rule group that your own rule group is copied from. To determine the update token for the managed rule group, call <a href=\\\"https://docs.aws.amazon.com/network-firewall/latest/APIReference/API_DescribeRuleGroup.html#networkfirewall-DescribeRuleGroup-response-UpdateToken\\\">DescribeRuleGroup</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-source-metadata-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: SourceMetadata
---
