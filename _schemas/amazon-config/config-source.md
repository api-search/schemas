---
description: Provides the CustomPolicyDetails, the rule owner (<code>Amazon Web Services</code> for managed rules, <code>CUSTOM_POLICY</code> for Custom Policy rules, and <code>CUSTOM_LAMBDA</code> for Custom Lambda rules), the rule identifier, and the events that cause the evaluation of your Amazon Web Services resources.
layout: schema
name: Source
properties_list:
- description: ''
  name: Owner
  type: object
- description: ''
  name: SourceIdentifier
  type: object
- description: ''
  name: SourceDetails
  type: object
- description: ''
  name: CustomPolicyDetails
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-source-schema.json
slug: config-source
source_filename: config-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-source-schema.json\",\n  \"title\": \"Source\",\n  \"description\": \"Provides the CustomPolicyDetails, the rule owner (<code>Amazon Web Services</code> for managed rules, <code>CUSTOM_POLICY</code> for Custom Policy rules, and <code>CUSTOM_LAMBDA</code> for Custom Lambda rules), the rule identifier, and the events that cause the evaluation of your Amazon Web Services resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Owner\"\n        },\n        {\n          \"description\": \"<p>Indicates whether Amazon Web Services or the customer owns and manages the Config rule.</p> <p>Config Managed Rules are predefined rules owned by Amazon Web Services. For more information, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config_use-managed-rules.html\\\
  \">Config Managed Rules</a> in the <i>Config developer guide</i>.</p> <p>Config Custom Rules are rules that you can develop either with Guard (<code>CUSTOM_POLICY</code>) or Lambda (<code>CUSTOM_LAMBDA</code>). For more information, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config_develop-rules.html\\\">Config Custom Rules </a> in the <i>Config developer guide</i>.</p>\"\n        }\n      ]\n    },\n    \"SourceIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"<p>For Config Managed rules, a predefined identifier from a list. For example, <code>IAM_PASSWORD_POLICY</code> is a managed rule. To reference a managed rule, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/managed-rules-by-aws-config.html\\\">List of Config Managed Rules</a>.</p> <p>For Config Custom Lambda rules, the identifier is the Amazon Resource\
  \ Name (ARN) of the rule's Lambda function, such as <code>arn:aws:lambda:us-east-2:123456789012:function:custom_rule_name</code>.</p> <p>For Config Custom Policy rules, this field will be ignored.</p>\"\n        }\n      ]\n    },\n    \"SourceDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceDetails\"\n        },\n        {\n          \"description\": \"<p>Provides the source and the message types that cause Config to evaluate your Amazon Web Services resources against a rule. It also provides the frequency with which you want Config to run evaluations for the rule if the trigger type is periodic.</p> <p>If the owner is set to <code>CUSTOM_POLICY</code>, the only acceptable values for the Config rule trigger message type are <code>ConfigurationItemChangeNotification</code> and <code>OversizedConfigurationItemChangeNotification</code>.</p>\"\n        }\n      ]\n    },\n    \"CustomPolicyDetails\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/CustomPolicyDetails\"\n        },\n        {\n          \"description\": \"Provides the runtime system, policy definition, and whether debug logging is enabled. Required when owner is set to <code>CUSTOM_POLICY</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Owner\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-source-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: Source
---
