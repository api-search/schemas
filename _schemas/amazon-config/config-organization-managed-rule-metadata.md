---
description: organization managed rule metadata such as resource type and ID of Amazon Web Services resource along with the rule identifier. It also provides the frequency with which you want Config to run evaluations for the rule if the trigger type is periodic.
layout: schema
name: OrganizationManagedRuleMetadata
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: RuleIdentifier
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
schema_file: json-schema/config-organization-managed-rule-metadata-schema.json
slug: config-organization-managed-rule-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-managed-rule-metadata-schema.json\",\n  \"title\": \"OrganizationManagedRuleMetadata\",\n  \"description\": \" organization managed rule metadata such as resource type and ID of Amazon Web Services resource along with the rule identifier. It also provides the frequency with which you want Config to run evaluations for the rule if the trigger type is periodic.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256Min0\"\n        },\n        {\n          \"description\": \"The description that you provide for your organization Config rule.\"\n        }\n      ]\n    },\n    \"RuleIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\
  \n        },\n        {\n          \"description\": \"For organization config managed rules, a predefined identifier from a list. For example, <code>IAM_PASSWORD_POLICY</code> is a managed rule. To reference a managed rule, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/evaluate-config_use-managed-rules.html\\\">Using Config managed rules</a>.\"\n        }\n      ]\n    },\n    \"InputParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit2048\"\n        },\n        {\n          \"description\": \"A string, in JSON format, that is passed to your organization Config rule Lambda function.\"\n        }\n      ]\n    },\n    \"MaximumExecutionFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumExecutionFrequency\"\n        },\n        {\n          \"description\": \"<p>The maximum frequency with which Config runs evaluations for a rule. This is for an Config managed\
  \ rule that is triggered at a periodic frequency.</p> <note> <p>By default, rules with a periodic trigger are evaluated every 24 hours. To change the frequency, specify a valid value for the <code>MaximumExecutionFrequency</code> parameter.</p> </note>\"\n        }\n      ]\n    },\n    \"ResourceTypesScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTypesScope\"\n        },\n        {\n          \"description\": \"The type of the Amazon Web Services resource that was evaluated.\"\n        }\n      ]\n    },\n    \"ResourceIdScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit768\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services resource that was evaluated.\"\n        }\n      ]\n    },\n    \"TagKeyScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit128\"\n        },\n        {\n          \"description\"\
  : \"One part of a key-value pair that make up a tag. A key is a general label that acts like a category for more specific tag values. \"\n        }\n      ]\n    },\n    \"TagValueScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The optional part of a key-value pair that make up a tag. A value acts as a descriptor within a tag category (key).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RuleIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-managed-rule-metadata-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: OrganizationManagedRuleMetadata
---
