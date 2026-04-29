---
description: A setting that enables metrics at the object level. Each rule contains an object group and an object group name. If the policy includes the MetricPolicyRules parameter, you must include at least one rule. Each metric policy can include up to five rules by default. You can also <a href="https://console.aws.amazon.com/servicequotas/home?region=us-east-1#!/services/mediastore/quotas">request a quota increase</a> to allow up to 300 rules per policy.
layout: schema
name: MetricPolicyRule
properties_list:
- description: ''
  name: ObjectGroup
  type: object
- description: ''
  name: ObjectGroupName
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-metric-policy-rule-schema.json
slug: mediastore-api-metric-policy-rule
source_filename: mediastore-api-metric-policy-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-metric-policy-rule-schema.json\",\n  \"title\": \"MetricPolicyRule\",\n  \"description\": \"A setting that enables metrics at the object level. Each rule contains an object group and an object group name. If the policy includes the MetricPolicyRules parameter, you must include at least one rule. Each metric policy can include up to five rules by default. You can also <a href=\\\"https://console.aws.amazon.com/servicequotas/home?region=us-east-1#!/services/mediastore/quotas\\\">request a quota increase</a> to allow up to 300 rules per policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ObjectGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectGroup\"\n        },\n        {\n          \"description\": \"A path or file name that defines\
  \ which objects to include in the group. Wildcards (*) are acceptable.\"\n        }\n      ]\n    },\n    \"ObjectGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectGroupName\"\n        },\n        {\n          \"description\": \"A name that allows you to refer to the object group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ObjectGroup\",\n    \"ObjectGroupName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-metric-policy-rule-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MetricPolicyRule
---
