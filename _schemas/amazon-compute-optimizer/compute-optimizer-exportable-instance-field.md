---
description: ExportableInstanceField schema
layout: schema
name: ExportableInstanceField
properties_list: []
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-exportable-instance-field-schema.json
slug: compute-optimizer-exportable-instance-field
source_filename: compute-optimizer-exportable-instance-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-exportable-instance-field-schema.json\",\n  \"title\": \"ExportableInstanceField\",\n  \"description\": \"ExportableInstanceField schema\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AccountId\",\n    \"InstanceArn\",\n    \"InstanceName\",\n    \"Finding\",\n    \"FindingReasonCodes\",\n    \"LookbackPeriodInDays\",\n    \"CurrentInstanceType\",\n    \"UtilizationMetricsCpuMaximum\",\n    \"UtilizationMetricsMemoryMaximum\",\n    \"UtilizationMetricsEbsReadOpsPerSecondMaximum\",\n    \"UtilizationMetricsEbsWriteOpsPerSecondMaximum\",\n    \"UtilizationMetricsEbsReadBytesPerSecondMaximum\",\n    \"UtilizationMetricsEbsWriteBytesPerSecondMaximum\",\n    \"UtilizationMetricsDiskReadOpsPerSecondMaximum\",\n    \"UtilizationMetricsDiskWriteOpsPerSecondMaximum\",\n    \"UtilizationMetricsDiskReadBytesPerSecondMaximum\"\
  ,\n    \"UtilizationMetricsDiskWriteBytesPerSecondMaximum\",\n    \"UtilizationMetricsNetworkInBytesPerSecondMaximum\",\n    \"UtilizationMetricsNetworkOutBytesPerSecondMaximum\",\n    \"UtilizationMetricsNetworkPacketsInPerSecondMaximum\",\n    \"UtilizationMetricsNetworkPacketsOutPerSecondMaximum\",\n    \"CurrentOnDemandPrice\",\n    \"CurrentStandardOneYearNoUpfrontReservedPrice\",\n    \"CurrentStandardThreeYearNoUpfrontReservedPrice\",\n    \"CurrentVCpus\",\n    \"CurrentMemory\",\n    \"CurrentStorage\",\n    \"CurrentNetwork\",\n    \"RecommendationOptionsInstanceType\",\n    \"RecommendationOptionsProjectedUtilizationMetricsCpuMaximum\",\n    \"RecommendationOptionsProjectedUtilizationMetricsMemoryMaximum\",\n    \"RecommendationOptionsPlatformDifferences\",\n    \"RecommendationOptionsPerformanceRisk\",\n    \"RecommendationOptionsVcpus\",\n    \"RecommendationOptionsMemory\",\n    \"RecommendationOptionsStorage\",\n    \"RecommendationOptionsNetwork\",\n    \"RecommendationOptionsOnDemandPrice\"\
  ,\n    \"RecommendationOptionsStandardOneYearNoUpfrontReservedPrice\",\n    \"RecommendationOptionsStandardThreeYearNoUpfrontReservedPrice\",\n    \"RecommendationsSourcesRecommendationSourceArn\",\n    \"RecommendationsSourcesRecommendationSourceType\",\n    \"LastRefreshTimestamp\",\n    \"CurrentPerformanceRisk\",\n    \"RecommendationOptionsSavingsOpportunityPercentage\",\n    \"RecommendationOptionsEstimatedMonthlySavingsCurrency\",\n    \"RecommendationOptionsEstimatedMonthlySavingsValue\",\n    \"EffectiveRecommendationPreferencesCpuVendorArchitectures\",\n    \"EffectiveRecommendationPreferencesEnhancedInfrastructureMetrics\",\n    \"EffectiveRecommendationPreferencesInferredWorkloadTypes\",\n    \"InferredWorkloadTypes\",\n    \"RecommendationOptionsMigrationEffort\",\n    \"EffectiveRecommendationPreferencesExternalMetricsSource\",\n    \"InstanceState\",\n    \"Tags\",\n    \"ExternalMetricStatusCode\",\n    \"ExternalMetricStatusReason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-exportable-instance-field-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ExportableInstanceField
---
