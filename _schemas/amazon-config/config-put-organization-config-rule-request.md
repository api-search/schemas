---
description: PutOrganizationConfigRuleRequest schema
layout: schema
name: PutOrganizationConfigRuleRequest
properties_list:
- description: ''
  name: OrganizationConfigRuleName
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
  name: OrganizationCustomPolicyRuleMetadata
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-organization-config-rule-request-schema.json
slug: config-put-organization-config-rule-request
source_filename: config-put-organization-config-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-organization-config-rule-request-schema.json\",\n  \"title\": \"PutOrganizationConfigRuleRequest\",\n  \"description\": \"PutOrganizationConfigRuleRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConfigRuleName\"\n        },\n        {\n          \"description\": \"The name that you assign to an organization Config rule.\"\n        }\n      ]\n    },\n    \"OrganizationManagedRuleMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationManagedRuleMetadata\"\n        },\n        {\n          \"description\": \"An <code>OrganizationManagedRuleMetadata</code> object. This object specifies organization managed rule\
  \ metadata such as resource type and ID of Amazon Web Services resource along with the rule identifier. It also provides the frequency with which you want Config to run evaluations for the rule if the trigger type is periodic.\"\n        }\n      ]\n    },\n    \"OrganizationCustomRuleMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationCustomRuleMetadata\"\n        },\n        {\n          \"description\": \"An <code>OrganizationCustomRuleMetadata</code> object. This object specifies organization custom rule metadata such as resource type, resource ID of Amazon Web Services resource, Lambda function ARN, and organization trigger types that trigger Config to evaluate your Amazon Web Services resources against a rule. It also provides the frequency with which you want Config to run evaluations for the rule if the trigger type is periodic.\"\n        }\n      ]\n    },\n    \"ExcludedAccounts\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/ExcludedAccounts\"\n        },\n        {\n          \"description\": \"A comma-separated list of accounts that you want to exclude from an organization Config rule.\"\n        }\n      ]\n    },\n    \"OrganizationCustomPolicyRuleMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationCustomPolicyRuleMetadata\"\n        },\n        {\n          \"description\": \"An <code>OrganizationCustomPolicyRuleMetadata</code> object. This object specifies metadata for your organization's Config Custom Policy rule. The metadata includes the runtime system in use, which accounts have debug logging enabled, and other custom rule metadata, such as resource type, resource ID of Amazon Web Services resource, and organization trigger types that initiate Config to evaluate Amazon Web Services resources against a rule.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OrganizationConfigRuleName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-organization-config-rule-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutOrganizationConfigRuleRequest
---
