---
description: Provides the runtime system, policy definition, and whether debug logging enabled. You can specify the following CustomPolicyDetails parameter values only for Config Custom Policy rules.
layout: schema
name: CustomPolicyDetails
properties_list:
- description: ''
  name: PolicyRuntime
  type: object
- description: ''
  name: PolicyText
  type: object
- description: ''
  name: EnableDebugLogDelivery
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-custom-policy-details-schema.json
slug: config-custom-policy-details
source_filename: config-custom-policy-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-custom-policy-details-schema.json\",\n  \"title\": \"CustomPolicyDetails\",\n  \"description\": \"Provides the runtime system, policy definition, and whether debug logging enabled. You can specify the following CustomPolicyDetails parameter values only for Config Custom Policy rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyRuntime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRuntime\"\n        },\n        {\n          \"description\": \"The runtime system for your Config Custom Policy rule. Guard is a policy-as-code language that allows you to write policies that are enforced by Config Custom Policy rules. For more information about Guard, see the <a href=\\\"https://github.com/aws-cloudformation/cloudformation-guard\\\">Guard GitHub Repository</a>.\"\
  \n        }\n      ]\n    },\n    \"PolicyText\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyText\"\n        },\n        {\n          \"description\": \"The policy definition containing the logic for your Config Custom Policy rule.\"\n        }\n      ]\n    },\n    \"EnableDebugLogDelivery\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The boolean expression for enabling debug logging for your Config Custom Policy rule. The default value is <code>false</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PolicyRuntime\",\n    \"PolicyText\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-custom-policy-details-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: CustomPolicyDetails
---
