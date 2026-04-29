---
description: <p>Indicates whether an Config rule is compliant based on account ID, region, compliance, and rule name.</p> <p>A rule is compliant if all of the resources that the rule evaluated comply with it. It is noncompliant if any of these resources do not comply.</p>
layout: schema
name: AggregateComplianceByConfigRule
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: Compliance
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: AwsRegion
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-aggregate-compliance-by-config-rule-schema.json
slug: config-aggregate-compliance-by-config-rule
source_filename: config-aggregate-compliance-by-config-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-compliance-by-config-rule-schema.json\",\n  \"title\": \"AggregateComplianceByConfigRule\",\n  \"description\": \"<p>Indicates whether an Config rule is compliant based on account ID, region, compliance, and rule name.</p> <p>A rule is compliant if all of the resources that the rule evaluated comply with it. It is noncompliant if any of these resources do not comply.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"The name of the Config rule.\"\n        }\n      ]\n    },\n    \"Compliance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Compliance\"\n        },\n        {\n        \
  \  \"description\": \"Indicates whether an Amazon Web Services resource or Config rule is compliant and provides the number of contributors that affect the compliance.\"\n        }\n      ]\n    },\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the source account.\"\n        }\n      ]\n    },\n    \"AwsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The source region from where the data is aggregated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregate-compliance-by-config-rule-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: AggregateComplianceByConfigRule
---
