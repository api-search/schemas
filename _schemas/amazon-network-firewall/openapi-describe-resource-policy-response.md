---
description: DescribeResourcePolicyResponse schema from Amazon Network Firewall
layout: schema
name: DescribeResourcePolicyResponse
properties_list:
- description: ''
  name: Policy
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-describe-resource-policy-response-schema.json
slug: openapi-describe-resource-policy-response
source_filename: openapi-describe-resource-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-resource-policy-response-schema.json\",\n  \"title\": \"DescribeResourcePolicyResponse\",\n  \"description\": \"DescribeResourcePolicyResponse schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyString\"\n        },\n        {\n          \"description\": \"The IAM policy for the resource. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-describe-resource-policy-response-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: DescribeResourcePolicyResponse
---
