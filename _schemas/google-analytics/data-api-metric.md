---
description: The quantitative measurements of a report. For example, the metric `eventCount` is the total number of events. Requests are allowed up to 10 metrics.
layout: schema
name: Metric
properties_list:
- description: A mathematical expression for derived metrics. For example, the metric Event count per user is `eventCount/totalUsers`.
  name: expression
  type: string
- description: Indicates if a metric is invisible in the report response. If a metric is invisible, the metric will not produce a column in the response, but can be used in `metricFilter`, `orderBys`, or a metric `e
  name: invisible
  type: boolean
- description: The name of the metric. See the [API Metrics](https://developers.google.com/analytics/devguides/reporting/data/v1/api-schema#metrics) for the list of metric names supported by core reporting methods s
  name: name
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/data-api-metric-schema.json
slug: data-api-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-metric-schema.json\",\n  \"title\": \"Metric\",\n  \"description\": \"The quantitative measurements of a report. For example, the metric `eventCount` is the total number of events. Requests are allowed up to 10 metrics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expression\": {\n      \"description\": \"A mathematical expression for derived metrics. For example, the metric Event count per user is `eventCount/totalUsers`.\",\n      \"type\": \"string\"\n    },\n    \"invisible\": {\n      \"description\": \"Indicates if a metric is invisible in the report response. If a metric is invisible, the metric will not produce a column in the response, but can be used in `metricFilter`, `orderBys`, or a metric `expression`.\",\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"\
  description\": \"The name of the metric. See the [API Metrics](https://developers.google.com/analytics/devguides/reporting/data/v1/api-schema#metrics) for the list of metric names supported by core reporting methods such as `runReport` and `batchRunReports`. See [Realtime Metrics](https://developers.google.com/analytics/devguides/reporting/data/v1/realtime-api-schema#metrics) for the list of metric names supported by the `runRealtimeReport` method. See [Funnel Metrics](https://developers.google.com/analytics/devguides/reporting/data/v1/exploration-api-schema#metrics) for the list of metric names supported by the `runFunnelReport` method. If `expression` is specified, `name` can be any string that you would like within the allowed character set. For example if `expression` is `screenPageViews/sessions`, you could call that metric's name = `viewsPerSession`. Metric names that you choose must match the regular expression `^[a-zA-Z0-9_]$`. Metrics are referenced by `name` in `metricFilter`,\
  \ `orderBys`, and metric `expression`.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-metric-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: Metric
---
