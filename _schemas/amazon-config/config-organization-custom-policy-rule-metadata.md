---
description: An object that specifies metadata for your organization's Config Custom Policy rule. The metadata includes the runtime system in use, which accounts have debug logging enabled, and other custom rule metadata, such as resource type, resource ID of Amazon Web Services resource, and organization trigger types that initiate Config to evaluate Amazon Web Services resources against a rule.
layout: schema
name: OrganizationCustomPolicyRuleMetadata
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: OrganizationConfigRuleTriggerTypes
  type: object
- description: ''
  name: InputParameters
  type: object
- description: ''
  name: MaximumExecutionFrequency
  type: object
- description: ''
  name: ResourceTypesScope
  type: object
- description: ''
  name: ResourceIdScope
  type: object
- description: ''
  name: TagKeyScope
  type: object
- description: ''
  name: TagValueScope
  type: object
- description: ''
  name: PolicyRuntime
  type: object
- description: ''
  name: PolicyText
  type: object
- description: ''
  name: DebugLogDeliveryAccounts
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-organization-custom-policy-rule-metadata-schema.json
slug: config-organization-custom-policy-rule-metadata
source_filename: config-organization-custom-policy-rule-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-custom-policy-rule-metadata-schema.json\",\n  \"title\": \"OrganizationCustomPolicyRuleMetadata\",\n  \"description\": \"An object that specifies metadata for your organization's Config Custom Policy rule. The metadata includes the runtime system in use, which accounts have debug logging enabled, and other custom rule metadata, such as resource type, resource ID of Amazon Web Services resource, and organization trigger types that initiate Config to evaluate Amazon Web Services resources against a rule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256Min0\"\n        },\n        {\n          \"description\": \"The description that you provide for your organization Config\
  \ Custom Policy rule.\"\n        }\n      ]\n    },\n    \"OrganizationConfigRuleTriggerTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConfigRuleTriggerTypeNoSNs\"\n        },\n        {\n          \"description\": \"<p>The type of notification that initiates Config to run an evaluation for a rule. For Config Custom Policy rules, Config supports change-initiated notification types:</p> <ul> <li> <p> <code>ConfigurationItemChangeNotification</code> - Initiates an evaluation when Config delivers a configuration item as a result of a resource change.</p> </li> <li> <p> <code>OversizedConfigurationItemChangeNotification</code> - Initiates an evaluation when Config delivers an oversized configuration item. Config may generate this notification type when a resource changes and the notification exceeds the maximum size allowed by Amazon SNS.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"InputParameters\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit2048\"\n        },\n        {\n          \"description\": \"A string, in JSON format, that is passed to your organization Config Custom Policy rule.\"\n        }\n      ]\n    },\n    \"MaximumExecutionFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumExecutionFrequency\"\n        },\n        {\n          \"description\": \"The maximum frequency with which Config runs evaluations for a rule. Your Config Custom Policy rule is triggered when Config delivers the configuration snapshot. For more information, see <a>ConfigSnapshotDeliveryProperties</a>.\"\n        }\n      ]\n    },\n    \"ResourceTypesScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTypesScope\"\n        },\n        {\n          \"description\": \"The type of the Amazon Web Services resource that was evaluated.\"\n        }\n      ]\n    },\n    \"ResourceIdScope\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit768\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services resource that was evaluated.\"\n        }\n      ]\n    },\n    \"TagKeyScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit128\"\n        },\n        {\n          \"description\": \"One part of a key-value pair that make up a tag. A key is a general label that acts like a category for more specific tag values.\"\n        }\n      ]\n    },\n    \"TagValueScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The optional part of a key-value pair that make up a tag. A value acts as a descriptor within a tag category (key).\"\n        }\n      ]\n    },\n    \"PolicyRuntime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyRuntime\"\
  \n        },\n        {\n          \"description\": \"The runtime system for your organization Config Custom Policy rules. Guard is a policy-as-code language that allows you to write policies that are enforced by Config Custom Policy rules. For more information about Guard, see the <a href=\\\"https://github.com/aws-cloudformation/cloudformation-guard\\\">Guard GitHub Repository</a>.\"\n        }\n      ]\n    },\n    \"PolicyText\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyText\"\n        },\n        {\n          \"description\": \"The policy definition containing the logic for your organization Config Custom Policy rule.\"\n        }\n      ]\n    },\n    \"DebugLogDeliveryAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DebugLogDeliveryAccounts\"\n        },\n        {\n          \"description\": \"A list of accounts that you can enable debug logging for your organization Config Custom Policy rule. List\
  \ is null when debug logging is enabled for all accounts.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PolicyRuntime\",\n    \"PolicyText\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-custom-policy-rule-metadata-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: OrganizationCustomPolicyRuleMetadata
---
