---
description: A single query to be processed. Use these parameters to query the Performance Insights GetResourceMetrics API to retrieve the metrics for an anomaly. For more information, see GetResourceMetrics in the Amazon RDS Performance Insights API Reference. Amazon RDS Performance Insights enables you to mo
layout: schema
name: PerformanceInsightsMetricQuery
properties_list:
- description: ''
  name: Metric
  type: object
- description: ''
  name: GroupBy
  type: object
- description: ''
  name: Filter
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-performance-insights-metric-query-schema.json
slug: amazon-devops-guru-performance-insights-metric-query
source_filename: amazon-devops-guru-performance-insights-metric-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-performance-insights-metric-query-schema.json\",\n  \"title\": \"PerformanceInsightsMetricQuery\",\n  \"description\": \"A single query to be processed. Use these parameters to query the Performance Insights GetResourceMetrics API to retrieve the metrics for an anomaly. For more information, see  GetResourceMetrics  in the Amazon RDS Performance Insights API Reference. Amazon RDS Performance Insights enables you to mo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Metric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PerformanceInsightsMetricName\"\n        },\n        {\n          \"description\": \"<p>The name of the meteric used used when querying an Performance Insights <code>GetResourceMetrics</code> API for anomaly metrics.</p> <p>Valid\
  \ values for <code>Metric</code> are:</p> <ul> <li> <p> <code>db.load.avg</code> - a scaled representation of the number of active sessions for the database engine.</p> </li> <li> <p> <code>db.sampledload.avg</code> - the raw number of active sessions for the database engine.</p> </li> </ul> <p>If the number of active sessions is less than an internal Performance Insights threshold, <code>db.load.avg</code> and <code>db.sampledload.avg</code> are the same value. If the number of active sessions is greater than the internal threshold, Performance Insights samples the active sessions, with <code>db.load.avg</code> showing the scaled values, <code>db.sampledload.avg</code> showing the raw values, and <code>db.sampledload.avg</code> less than <code>db.load.avg</code>. For most use cases, you can query <code>db.load.avg</code> only. </p>\"\n        }\n      ]\n    },\n    \"GroupBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PerformanceInsightsMetricDimensionGroup\"\
  \n        },\n        {\n          \"description\": \"The specification for how to aggregate the data points from a Performance Insights <code>GetResourceMetrics</code> API query. The Performance Insights query returns all of the dimensions within that group, unless you provide the names of specific dimensions within that group. You can also request that Performance Insights return a limited number of values for a dimension.\"\n        }\n      ]\n    },\n    \"Filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PerformanceInsightsMetricFilterMap\"\n        },\n        {\n          \"description\": \"<p>One or more filters to apply to a Performance Insights <code>GetResourceMetrics</code> API query. Restrictions:</p> <ul> <li> <p>Any number of filters by the same dimension, as specified in the <code>GroupBy</code> parameter.</p> </li> <li> <p>A single filter for any other dimension in this dimension group.</p> </li> </ul>\"\n        }\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-performance-insights-metric-query-schema.json
tags:
- Anomaly Detection
- DevOps
- Machine Learning
- Operational Intelligence
title: PerformanceInsightsMetricQuery
---
