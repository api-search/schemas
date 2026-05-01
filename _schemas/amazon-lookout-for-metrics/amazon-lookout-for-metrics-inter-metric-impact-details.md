---
description: <p>Aggregated details about the measures contributing to the anomaly group, and the measures potentially impacted by the anomaly group.</p> <p/>
layout: schema
name: InterMetricImpactDetails
properties_list:
- description: ''
  name: MetricName
  type: object
- description: ''
  name: AnomalyGroupId
  type: object
- description: ''
  name: RelationshipType
  type: object
- description: ''
  name: ContributionPercentage
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-inter-metric-impact-details-schema.json
slug: amazon-lookout-for-metrics-inter-metric-impact-details
source_filename: amazon-lookout-for-metrics-inter-metric-impact-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-inter-metric-impact-details-schema.json\",\n  \"title\": \"InterMetricImpactDetails\",\n  \"description\": \"<p>Aggregated details about the measures contributing to the anomaly group, and the measures potentially impacted by the anomaly group.</p> <p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricName\"\n        },\n        {\n          \"description\": \"The name of the measure.\"\n        }\n      ]\n    },\n    \"AnomalyGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n          \"description\": \"The ID of the anomaly group.\"\n        }\n      ]\n    },\n    \"RelationshipType\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelationshipType\"\n        },\n        {\n          \"description\": \"Whether a measure is a potential cause of the anomaly group (<code>CAUSE_OF_INPUT_ANOMALY_GROUP</code>), or whether the measure is impacted by the anomaly group (<code>EFFECT_OF_INPUT_ANOMALY_GROUP</code>).\"\n        }\n      ]\n    },\n    \"ContributionPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricChangePercentage\"\n        },\n        {\n          \"description\": \"For potential causes (<code>CAUSE_OF_INPUT_ANOMALY_GROUP</code>), the percentage contribution the measure has in causing the anomalies.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-inter-metric-impact-details-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: InterMetricImpactDetails
---
