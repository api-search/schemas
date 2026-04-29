---
description: Schema representing an AppDynamics health rule configuration that defines performance thresholds, violation conditions, and evaluation criteria for monitored entities.
layout: schema
name: AppDynamics Health Rule
properties_list:
- description: The internal numeric identifier for the health rule.
  name: id
  type: integer
- description: The name of the health rule.
  name: name
  type: string
- description: Whether the health rule is currently enabled.
  name: enabled
  type: boolean
- description: The evaluation time window in minutes.
  name: useDataFromLastNMinutes
  type: integer
- description: Time in minutes to wait after a violation before re-evaluating.
  name: waitTimeAfterViolation
  type: integer
- description: The schedule name that determines when this health rule is active.
  name: scheduleName
  type: string
- description: Defines which entities are affected by this health rule.
  name: affects
  type: object
- description: The evaluation criteria containing critical and warning conditions.
  name: evalCriterias
  type: object
provider_name: AppDynamics
provider_slug: appdynamics
schema_file: json-schema/appdynamics-health-rule-schema.json
slug: appdynamics-health-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://appdynamics.com/schemas/appdynamics/health-rule.json\",\n  \"title\": \"AppDynamics Health Rule\",\n  \"description\": \"Schema representing an AppDynamics health rule configuration that defines performance thresholds, violation conditions, and evaluation criteria for monitored entities.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"enabled\", \"affects\", \"evalCriterias\"],\n  \"$defs\": {\n    \"MetricCondition\": {\n      \"type\": \"object\",\n      \"description\": \"A metric evaluation condition that defines a threshold for triggering a violation.\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of condition evaluation.\",\n          \"enum\": [\n            \"SINGLE_METRIC\",\n            \"METRIC_EXPRESSION\"\n          ]\n        },\n        \"metricPath\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"The metric path to evaluate using pipe-delimited hierarchy.\"\n        },\n        \"operator\": {\n          \"type\": \"string\",\n          \"description\": \"The comparison operator for the threshold.\",\n          \"enum\": [\n            \"GREATER_THAN\",\n            \"LESS_THAN\",\n            \"GREATER_THAN_EQUALS\",\n            \"LESS_THAN_EQUALS\",\n            \"EQUALS\",\n            \"NOT_EQUALS\"\n          ]\n        },\n        \"value\": {\n          \"type\": \"number\",\n          \"description\": \"The threshold value for comparison.\"\n        },\n        \"useActiveBaseline\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to use the active baseline for dynamic threshold calculation.\"\n        },\n        \"baselineDeviation\": {\n          \"type\": \"string\",\n          \"description\": \"The baseline deviation direction for dynamic thresholds.\",\n          \"enum\": [\n\
  \            \"ABOVE\",\n            \"BELOW\",\n            \"ABOVE_OR_BELOW\"\n          ]\n        },\n        \"baselineDeviations\": {\n          \"type\": \"number\",\n          \"description\": \"The number of standard deviations from baseline to trigger a violation.\",\n          \"minimum\": 0\n        }\n      }\n    }\n  },\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The internal numeric identifier for the health rule.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the health rule.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the health rule is currently enabled.\"\n    },\n    \"useDataFromLastNMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The evaluation time window in minutes.\",\n      \"minimum\": 1,\n      \"maximum\": 1440\n    },\n    \"waitTimeAfterViolation\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Time in minutes to wait after a violation before re-evaluating.\",\n      \"minimum\": 0\n    },\n    \"scheduleName\": {\n      \"type\": \"string\",\n      \"description\": \"The schedule name that determines when this health rule is active.\",\n      \"default\": \"Always\"\n    },\n    \"affects\": {\n      \"type\": \"object\",\n      \"description\": \"Defines which entities are affected by this health rule.\",\n      \"required\": [\"affectedEntityType\"],\n      \"properties\": {\n        \"affectedEntityType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of entity this health rule evaluates.\",\n          \"enum\": [\n            \"OVERALL_APPLICATION\",\n            \"BUSINESS_TRANSACTION\",\n            \"TIER_NODE\",\n            \"BACKEND\",\n            \"INFORMATION_POINT\",\n            \"CUSTOM\",\n            \"MOBILE_APPLICATION\",\n            \"BROWSER_APPLICATION\"\n        \
  \  ]\n        },\n        \"affectedBusinessTransactions\": {\n          \"type\": \"object\",\n          \"description\": \"Business transaction selection criteria.\",\n          \"properties\": {\n            \"businessTransactionScope\": {\n              \"type\": \"string\",\n              \"description\": \"The scope for selecting business transactions.\",\n              \"enum\": [\n                \"ALL_BUSINESS_TRANSACTIONS\",\n                \"SPECIFIC_BUSINESS_TRANSACTIONS\",\n                \"BUSINESS_TRANSACTIONS_MATCHING_PATTERN\"\n              ]\n            }\n          }\n        },\n        \"affectedNodes\": {\n          \"type\": \"object\",\n          \"description\": \"Node selection criteria.\",\n          \"properties\": {\n            \"affectedNodeScope\": {\n              \"type\": \"string\",\n              \"description\": \"The scope for selecting nodes.\",\n              \"enum\": [\n                \"ALL_NODES\",\n                \"SPECIFIC_NODES\",\n\
  \                \"NODES_MATCHING_PATTERN\",\n                \"NODES_OF_SPECIFIC_TIERS\"\n              ]\n            }\n          }\n        }\n      }\n    },\n    \"evalCriterias\": {\n      \"type\": \"object\",\n      \"description\": \"The evaluation criteria containing critical and warning conditions.\",\n      \"properties\": {\n        \"criticalCriteria\": {\n          \"type\": \"object\",\n          \"description\": \"The critical severity evaluation criteria.\",\n          \"properties\": {\n            \"conditionAggregationType\": {\n              \"type\": \"string\",\n              \"description\": \"How to aggregate multiple conditions.\",\n              \"enum\": [\"ALL\", \"ANY\", \"CUSTOM\"]\n            },\n            \"conditions\": {\n              \"type\": \"array\",\n              \"description\": \"The list of metric conditions for critical violations.\",\n              \"items\": {\n                \"$ref\": \"#/$defs/MetricCondition\"\n              }\n\
  \            }\n          }\n        },\n        \"warningCriteria\": {\n          \"type\": \"object\",\n          \"description\": \"The warning severity evaluation criteria.\",\n          \"properties\": {\n            \"conditionAggregationType\": {\n              \"type\": \"string\",\n              \"description\": \"How to aggregate multiple conditions.\",\n              \"enum\": [\"ALL\", \"ANY\", \"CUSTOM\"]\n            },\n            \"conditions\": {\n              \"type\": \"array\",\n              \"description\": \"The list of metric conditions for warning violations.\",\n              \"items\": {\n                \"$ref\": \"#/$defs/MetricCondition\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/json-schema/appdynamics-health-rule-schema.json
tags:
- APM
- Application Performance Monitoring
- Cisco
- Cloud Observability
- DevOps
- Monitoring
- Observability
- OpenTelemetry
title: AppDynamics Health Rule
---
