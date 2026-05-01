---
description: <p>The metric policy that is associated with the container. A metric policy allows AWS Elemental MediaStore to send metrics to Amazon CloudWatch. In the policy, you must indicate whether you want MediaStore to send container-level metrics. You can also include rules to define groups of objects that you want MediaStore to send object-level metrics for.</p> <p>To view examples of how to construct a metric policy for your use case, see <a href="https://docs.aws.amazon.com/mediastore/latest/ug/policies-metric-examples.html">Example Metric Policies</a>.</p>
layout: schema
name: MetricPolicy
properties_list:
- description: ''
  name: ContainerLevelMetrics
  type: object
- description: ''
  name: MetricPolicyRules
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-metric-policy-schema.json
slug: mediastore-api-metric-policy
source_filename: mediastore-api-metric-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-metric-policy-schema.json\",\n  \"title\": \"MetricPolicy\",\n  \"description\": \"<p>The metric policy that is associated with the container. A metric policy allows AWS Elemental MediaStore to send metrics to Amazon CloudWatch. In the policy, you must indicate whether you want MediaStore to send container-level metrics. You can also include rules to define groups of objects that you want MediaStore to send object-level metrics for.</p> <p>To view examples of how to construct a metric policy for your use case, see <a href=\\\"https://docs.aws.amazon.com/mediastore/latest/ug/policies-metric-examples.html\\\">Example Metric Policies</a>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerLevelMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerLevelMetrics\"\
  \n        },\n        {\n          \"description\": \"A setting to enable or disable metrics at the container level.\"\n        }\n      ]\n    },\n    \"MetricPolicyRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricPolicyRules\"\n        },\n        {\n          \"description\": \"A parameter that holds an array of rules that enable metrics at the object level. This parameter is optional, but if you choose to include it, you must also include at least one rule. By default, you can include up to five rules. You can also <a href=\\\"https://console.aws.amazon.com/servicequotas/home?region=us-east-1#!/services/mediastore/quotas\\\">request a quota increase</a> to allow up to 300 rules per policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ContainerLevelMetrics\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-metric-policy-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MetricPolicy
---
