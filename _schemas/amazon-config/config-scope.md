---
description: Defines which resources trigger an evaluation for an Config rule. The scope can include one or more resource types, a combination of a tag key and value, or a combination of one resource type and one resource ID. Specify a scope to constrain which resources trigger an evaluation for a rule. Otherwise, evaluations for the rule are triggered when any resource in your recording group changes in configuration.
layout: schema
name: Scope
properties_list:
- description: ''
  name: ComplianceResourceTypes
  type: object
- description: ''
  name: TagKey
  type: object
- description: ''
  name: TagValue
  type: object
- description: ''
  name: ComplianceResourceId
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-scope-schema.json
slug: config-scope
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-scope-schema.json\",\n  \"title\": \"Scope\",\n  \"description\": \"Defines which resources trigger an evaluation for an Config rule. The scope can include one or more resource types, a combination of a tag key and value, or a combination of one resource type and one resource ID. Specify a scope to constrain which resources trigger an evaluation for a rule. Otherwise, evaluations for the rule are triggered when any resource in your recording group changes in configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComplianceResourceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceResourceTypes\"\n        },\n        {\n          \"description\": \"The resource types of only those Amazon Web Services resources that you want to trigger an\
  \ evaluation for the rule. You can only specify one type if you also specify a resource ID for <code>ComplianceResourceId</code>.\"\n        }\n      ]\n    },\n    \"TagKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit128\"\n        },\n        {\n          \"description\": \"The tag key that is applied to only those Amazon Web Services resources that you want to trigger an evaluation for the rule.\"\n        }\n      ]\n    },\n    \"TagValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The tag value applied to only those Amazon Web Services resources that you want to trigger an evaluation for the rule. If you specify a value for <code>TagValue</code>, you must also specify a value for <code>TagKey</code>.\"\n        }\n      ]\n    },\n    \"ComplianceResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/BaseResourceId\"\n        },\n        {\n          \"description\": \"The ID of the only Amazon Web Services resource that you want to trigger an evaluation for the rule. If you specify a resource ID, you must specify one resource type for <code>ComplianceResourceTypes</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-scope-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: Scope
---
