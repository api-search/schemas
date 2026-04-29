---
description: Describes a recommendation preference.
layout: schema
name: RecommendationPreferencesDetail
properties_list:
- description: ''
  name: scope
  type: object
- description: ''
  name: resourceType
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
schema_file: json-schema/compute-optimizer-recommendation-preferences-detail-schema.json
slug: compute-optimizer-recommendation-preferences-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommendation-preferences-detail-schema.json\",\n  \"title\": \"RecommendationPreferencesDetail\",\n  \"description\": \"Describes a recommendation preference.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scope\"\n        },\n        {\n          \"description\": \"<p>An object that describes the scope of the recommendation preference.</p> <p>Recommendation preferences can be created at the organization level (for management accounts of an organization only), account level, and resource level. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/enhanced-infrastructure-metrics.html\\\">Activating enhanced infrastructure metrics</a> in the\
  \ <i>Compute Optimizer User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"<p>The target resource type of the recommendation preference to create.</p> <p>The <code>Ec2Instance</code> option encompasses standalone instances and instances that are part of Auto Scaling groups. The <code>AutoScalingGroup</code> option encompasses only instances that are part of an Auto Scaling group.</p>\"\n        }\n      ]\n    },\n    \"enhancedInfrastructureMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnhancedInfrastructureMetrics\"\n        },\n        {\n          \"description\": \"<p>The status of the enhanced infrastructure metrics recommendation preference.</p> <p>When the recommendations page is refreshed, a status of <code>Active</code> confirms that the preference is applied to the recommendations,\
  \ and a status of <code>Inactive</code> confirms that the preference isn't yet applied to recommendations.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/enhanced-infrastructure-metrics.html\\\">Enhanced infrastructure metrics</a> in the <i>Compute Optimizer User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"inferredWorkloadTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferredWorkloadTypesPreference\"\n        },\n        {\n          \"description\": \"<p>The status of the inferred workload types recommendation preference.</p> <p>When the recommendations page is refreshed, a status of <code>Active</code> confirms that the preference is applied to the recommendations, and a status of <code>Inactive</code> confirms that the preference isn't yet applied to recommendations.</p>\"\n        }\n      ]\n    },\n    \"externalMetricsPreference\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/ExternalMetricsPreference\"\n        },\n        {\n          \"description\": \"<p> An object that describes the external metrics recommendation preference. </p> <p> If the preference is applied in the latest recommendation refresh, an object with a valid <code>source</code> value appears in the response. If the preference isn't applied to the recommendations already, then this object doesn't appear in the response. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommendation-preferences-detail-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: RecommendationPreferencesDetail
---
