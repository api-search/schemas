---
description: Describes the effective recommendation preferences for a resource.
layout: schema
name: EffectiveRecommendationPreferences
properties_list:
- description: ''
  name: cpuVendorArchitectures
  type: object
- description: ''
  name: enhancedInfrastructureMetrics
  type: object
- description: ''
  name: inferredWorkloadTypes
  type: object
- description: ''
  name: externalMetricsPreference
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-effective-recommendation-preferences-schema.json
slug: compute-optimizer-effective-recommendation-preferences
source_filename: compute-optimizer-effective-recommendation-preferences-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-effective-recommendation-preferences-schema.json\",\n  \"title\": \"EffectiveRecommendationPreferences\",\n  \"description\": \"Describes the effective recommendation preferences for a resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cpuVendorArchitectures\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CpuVendorArchitectures\"\n        },\n        {\n          \"description\": \"<p>Describes the CPU vendor and architecture for an instance or Auto Scaling group recommendations.</p> <p>For example, when you specify <code>AWS_ARM64</code> with:</p> <ul> <li> <p>A <a>GetEC2InstanceRecommendations</a> or <a>GetAutoScalingGroupRecommendations</a> request, Compute Optimizer returns recommendations that consist of Graviton2 instance types\
  \ only.</p> </li> <li> <p>A <a>GetEC2RecommendationProjectedMetrics</a> request, Compute Optimizer returns projected utilization metrics for Graviton2 instance type recommendations only.</p> </li> <li> <p>A <a>ExportEC2InstanceRecommendations</a> or <a>ExportAutoScalingGroupRecommendations</a> request, Compute Optimizer exports recommendations that consist of Graviton2 instance types only.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"enhancedInfrastructureMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnhancedInfrastructureMetrics\"\n        },\n        {\n          \"description\": \"<p>Describes the activation status of the enhanced infrastructure metrics preference.</p> <p>A status of <code>Active</code> confirms that the preference is applied in the latest recommendation refresh, and a status of <code>Inactive</code> confirms that it's not yet applied to recommendations.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/enhanced-infrastructure-metrics.html\\\
  \">Enhanced infrastructure metrics</a> in the <i>Compute Optimizer User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"inferredWorkloadTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferredWorkloadTypesPreference\"\n        },\n        {\n          \"description\": \"<p>Describes the activation status of the inferred workload types preference.</p> <p>A status of <code>Active</code> confirms that the preference is applied in the latest recommendation refresh. A status of <code>Inactive</code> confirms that it's not yet applied to recommendations.</p>\"\n        }\n      ]\n    },\n    \"externalMetricsPreference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalMetricsPreference\"\n        },\n        {\n          \"description\": \"<p> An object that describes the external metrics recommendation preference. </p> <p> If the preference is applied in the latest recommendation refresh, an object with a valid\
  \ <code>source</code> value appears in the response. If the preference isn't applied to the recommendations already, then this object doesn't appear in the response. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-effective-recommendation-preferences-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: EffectiveRecommendationPreferences
---
