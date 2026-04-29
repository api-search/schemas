---
description: An organization Config rule that has information about Config rules that Config creates in member accounts.
layout: schema
name: OrganizationConfigRule
properties_list:
- description: ''
  name: OrganizationConfigRuleName
  type: object
- description: ''
  name: OrganizationConfigRuleArn
  type: object
- description: ''
  name: OrganizationManagedRuleMetadata
  type: object
- description: ''
  name: OrganizationCustomRuleMetadata
  type: object
- description: ''
  name: ExcludedAccounts
  type: object
- description: ''
  name: LastUpdateTime
  type: object
- description: ''
  name: OrganizationCustomPolicyRuleMetadata
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-organization-config-rule-schema.json
slug: config-organization-config-rule
source_filename: config-organization-config-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-config-rule-schema.json\",\n  \"title\": \"OrganizationConfigRule\",\n  \"description\": \"An organization Config rule that has information about Config rules that Config creates in member accounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConfigRuleName\"\n        },\n        {\n          \"description\": \"The name that you assign to organization Config rule.\"\n        }\n      ]\n    },\n    \"OrganizationConfigRuleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of organization Config rule.\"\n        }\n     \
  \ ]\n    },\n    \"OrganizationManagedRuleMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationManagedRuleMetadata\"\n        },\n        {\n          \"description\": \"An <code>OrganizationManagedRuleMetadata</code> object.\"\n        }\n      ]\n    },\n    \"OrganizationCustomRuleMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationCustomRuleMetadata\"\n        },\n        {\n          \"description\": \"An <code>OrganizationCustomRuleMetadata</code> object.\"\n        }\n      ]\n    },\n    \"ExcludedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExcludedAccounts\"\n        },\n        {\n          \"description\": \"A comma-separated list of accounts excluded from organization Config rule.\"\n        }\n      ]\n    },\n    \"LastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n   \
  \     {\n          \"description\": \"The timestamp of the last update.\"\n        }\n      ]\n    },\n    \"OrganizationCustomPolicyRuleMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationCustomPolicyRuleMetadataNoPolicy\"\n        },\n        {\n          \"description\": \"An object that specifies metadata for your organization's Config Custom Policy rule. The metadata includes the runtime system in use, which accounts have debug logging enabled, and other custom rule metadata, such as resource type, resource ID of Amazon Web Services resource, and organization trigger types that initiate Config to evaluate Amazon Web Services resources against a rule.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OrganizationConfigRuleName\",\n    \"OrganizationConfigRuleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-config-rule-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: OrganizationConfigRule
---
