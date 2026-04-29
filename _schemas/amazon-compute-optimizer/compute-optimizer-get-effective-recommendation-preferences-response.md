---
description: GetEffectiveRecommendationPreferencesResponse schema
layout: schema
name: GetEffectiveRecommendationPreferencesResponse
properties_list:
- description: ''
  name: enhancedInfrastructureMetrics
  type: object
- description: ''
  name: externalMetricsPreference
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-effective-recommendation-preferences-response-schema.json
slug: compute-optimizer-get-effective-recommendation-preferences-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-effective-recommendation-preferences-response-schema.json\",\n  \"title\": \"GetEffectiveRecommendationPreferencesResponse\",\n  \"description\": \"GetEffectiveRecommendationPreferencesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enhancedInfrastructureMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnhancedInfrastructureMetrics\"\n        },\n        {\n          \"description\": \"<p>The status of the enhanced infrastructure metrics recommendation preference. Considers all applicable preferences that you might have set at the resource, account, and organization level.</p> <p>A status of <code>Active</code> confirms that the preference is applied in the latest recommendation refresh, and a status of <code>Inactive</code>\
  \ confirms that it's not yet applied to recommendations.</p> <p>To validate whether the preference is applied to your last generated set of recommendations, review the <code>effectiveRecommendationPreferences</code> value in the response of the <a>GetAutoScalingGroupRecommendations</a> and <a>GetEC2InstanceRecommendations</a> actions.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/enhanced-infrastructure-metrics.html\\\">Enhanced infrastructure metrics</a> in the <i>Compute Optimizer User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"externalMetricsPreference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalMetricsPreference\"\n        },\n        {\n          \"description\": \"<p>The provider of the external metrics recommendation preference. Considers all applicable preferences that you might have set at the account and organization level.</p> <p>If the preference is applied in the latest\
  \ recommendation refresh, an object with a valid <code>source</code> value appears in the response. If the preference isn't applied to the recommendations already, then this object doesn't appear in the response.</p> <p>To validate whether the preference is applied to your last generated set of recommendations, review the <code>effectiveRecommendationPreferences</code> value in the response of the <a>GetEC2InstanceRecommendations</a> actions.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/external-metrics-ingestion.html\\\">Enhanced infrastructure metrics</a> in the <i>Compute Optimizer User Guide</i>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-effective-recommendation-preferences-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetEffectiveRecommendationPreferencesResponse
---
