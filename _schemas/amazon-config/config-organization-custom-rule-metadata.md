---
description: organization custom rule metadata such as resource type, resource ID of Amazon Web Services resource, Lambda function ARN, and organization trigger types that trigger Config to evaluate your Amazon Web Services resources against a rule. It also provides the frequency with which you want Config to run evaluations for the rule if the trigger type is periodic.
layout: schema
name: OrganizationCustomRuleMetadata
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: LambdaFunctionArn
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
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-organization-custom-rule-metadata-schema.json
slug: config-organization-custom-rule-metadata
source_filename: config-organization-custom-rule-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-custom-rule-metadata-schema.json\",\n  \"title\": \"OrganizationCustomRuleMetadata\",\n  \"description\": \" organization custom rule metadata such as resource type, resource ID of Amazon Web Services resource, Lambda function ARN, and organization trigger types that trigger Config to evaluate your Amazon Web Services resources against a rule. It also provides the frequency with which you want Config to run evaluations for the rule if the trigger type is periodic.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256Min0\"\n        },\n        {\n          \"description\": \"The description that you provide for your organization Config rule.\"\n        }\n      ]\n    },\n\
  \    \"LambdaFunctionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The lambda function ARN.\"\n        }\n      ]\n    },\n    \"OrganizationConfigRuleTriggerTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConfigRuleTriggerTypes\"\n        },\n        {\n          \"description\": \"<p>The type of notification that triggers Config to run an evaluation for a rule. You can specify the following notification types:</p> <ul> <li> <p> <code>ConfigurationItemChangeNotification</code> - Triggers an evaluation when Config delivers a configuration item as a result of a resource change.</p> </li> <li> <p> <code>OversizedConfigurationItemChangeNotification</code> - Triggers an evaluation when Config delivers an oversized configuration item. Config may generate this notification type when a resource changes and the notification exceeds\
  \ the maximum size allowed by Amazon SNS.</p> </li> <li> <p> <code>ScheduledNotification</code> - Triggers a periodic evaluation at the frequency specified for <code>MaximumExecutionFrequency</code>.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"InputParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit2048\"\n        },\n        {\n          \"description\": \"A string, in JSON format, that is passed to your organization Config rule Lambda function.\"\n        }\n      ]\n    },\n    \"MaximumExecutionFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumExecutionFrequency\"\n        },\n        {\n          \"description\": \"<p>The maximum frequency with which Config runs evaluations for a rule. Your custom rule is triggered when Config delivers the configuration snapshot. For more information, see <a>ConfigSnapshotDeliveryProperties</a>.</p> <note> <p>By default, rules with a\
  \ periodic trigger are evaluated every 24 hours. To change the frequency, specify a valid value for the <code>MaximumExecutionFrequency</code> parameter.</p> </note>\"\n        }\n      ]\n    },\n    \"ResourceTypesScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTypesScope\"\n        },\n        {\n          \"description\": \"The type of the Amazon Web Services resource that was evaluated.\"\n        }\n      ]\n    },\n    \"ResourceIdScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit768\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services resource that was evaluated.\"\n        }\n      ]\n    },\n    \"TagKeyScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit128\"\n        },\n        {\n          \"description\": \"One part of a key-value pair that make up a tag. A key is a general label that\
  \ acts like a category for more specific tag values. \"\n        }\n      ]\n    },\n    \"TagValueScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The optional part of a key-value pair that make up a tag. A value acts as a descriptor within a tag category (key). \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LambdaFunctionArn\",\n    \"OrganizationConfigRuleTriggerTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-custom-rule-metadata-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: OrganizationCustomRuleMetadata
---
