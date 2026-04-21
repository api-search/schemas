---
description: ''
layout: schema
name: TimeSeriesServiceStatistics
properties_list:
- description: ''
  name: Timestamp
  type: string
- description: ''
  name: EdgeSummaryStatistics
  type: object
- description: ''
  name: ServiceSummaryStatistics
  type: object
- description: ''
  name: ServiceForecastStatistics
  type: object
- description: ''
  name: ResponseTimeHistogram
  type: array
provider_name: AWS X-Ray
provider_slug: aws-x-ray
schema_file: json-schema/x-ray-timeseriesservicestatistics-schema.json
slug: x-ray-timeseriesservicestatistics
tags:
- AWS
- Debugging
- Distributed Tracing
- Microservices
- Observability
title: TimeSeriesServiceStatistics
---
