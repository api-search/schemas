---
description: Describes the external metrics preferences for EC2 rightsizing recommendations.
layout: schema
name: ExternalMetricsPreference
properties_list:
- description: ''
  name: source
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-external-metrics-preference-schema.json
slug: compute-optimizer-external-metrics-preference
source_filename: compute-optimizer-external-metrics-preference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-external-metrics-preference-schema.json\",\n  \"title\": \"ExternalMetricsPreference\",\n  \"description\": \" Describes the external metrics preferences for EC2 rightsizing recommendations. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalMetricsSource\"\n        },\n        {\n          \"description\": \" Contains the source options for external metrics preferences. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-external-metrics-preference-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ExternalMetricsPreference
---
