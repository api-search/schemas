---
description: DescribeRuleGroupMetadataRequest schema from Amazon Network Firewall
layout: schema
name: DescribeRuleGroupMetadataRequest
properties_list:
- description: ''
  name: RuleGroupName
  type: object
- description: ''
  name: RuleGroupArn
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-describe-rule-group-metadata-request-schema.json
slug: openapi-describe-rule-group-metadata-request
source_filename: openapi-describe-rule-group-metadata-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-rule-group-metadata-request-schema.json\",\n  \"title\": \"DescribeRuleGroupMetadataRequest\",\n  \"description\": \"DescribeRuleGroupMetadataRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"<p>The descriptive name of the rule group. You can't change the name of a rule group after you create it.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    },\n    \"RuleGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"<p>The\
  \ descriptive name of the rule group. You can't change the name of a rule group after you create it.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupType\"\n        },\n        {\n          \"description\": \"<p>Indicates whether the rule group is stateless or stateful. If the rule group is stateless, it contains stateless rules. If it is stateful, it contains stateful rules. </p> <note> <p>This setting is required for requests that do not include the <code>RuleGroupARN</code>.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-rule-group-metadata-request-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: DescribeRuleGroupMetadataRequest
---
