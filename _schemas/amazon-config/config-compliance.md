---
description: Indicates whether an Amazon Web Services resource or Config rule is compliant and provides the number of contributors that affect the compliance.
layout: schema
name: Compliance
properties_list:
- description: ''
  name: ComplianceType
  type: object
- description: ''
  name: ComplianceContributorCount
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-compliance-schema.json
slug: config-compliance
source_filename: config-compliance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-schema.json\",\n  \"title\": \"Compliance\",\n  \"description\": \"Indicates whether an Amazon Web Services resource or Config rule is compliant and provides the number of contributors that affect the compliance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ComplianceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceType\"\n        },\n        {\n          \"description\": \"<p>Indicates whether an Amazon Web Services resource or Config rule is compliant.</p> <p>A resource is compliant if it complies with all of the Config rules that evaluate it. A resource is noncompliant if it does not comply with one or more of these rules.</p> <p>A rule is compliant if all of the resources that the rule evaluates comply with it. A rule is noncompliant\
  \ if any of these resources do not comply.</p> <p>Config returns the <code>INSUFFICIENT_DATA</code> value when no evaluation results are available for the Amazon Web Services resource or Config rule.</p> <p>For the <code>Compliance</code> data type, Config supports only <code>COMPLIANT</code>, <code>NON_COMPLIANT</code>, and <code>INSUFFICIENT_DATA</code> values. Config does not support the <code>NOT_APPLICABLE</code> value for the <code>Compliance</code> data type.</p>\"\n        }\n      ]\n    },\n    \"ComplianceContributorCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceContributorCount\"\n        },\n        {\n          \"description\": \"The number of Amazon Web Services resources or Config rules that cause a result of <code>NON_COMPLIANT</code>, up to a maximum number.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: Compliance
---
