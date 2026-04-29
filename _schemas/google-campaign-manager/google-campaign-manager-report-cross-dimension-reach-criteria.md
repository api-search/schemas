---
description: Configuration for a CROSS_DIMENSION_REACH report type.
layout: schema
name: ReportCrossDimensionReachCriteria
properties_list:
- description: ''
  name: dimension
  type: string
- description: ''
  name: metricNames
  type: array
- description: ''
  name: overlapMetricNames
  type: array
- description: ''
  name: dimensionFilters
  type: array
- description: ''
  name: pivoted
  type: boolean
- description: ''
  name: breakdown
  type: array
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-report-cross-dimension-reach-criteria-schema.json
slug: google-campaign-manager-report-cross-dimension-reach-criteria
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportCrossDimensionReachCriteria\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for a CROSS_DIMENSION_REACH report type.\",\n  \"properties\": {\n    \"dimension\": {\n      \"type\": \"string\"\n    },\n    \"metricNames\": {\n      \"type\": \"array\"\n    },\n    \"overlapMetricNames\": {\n      \"type\": \"array\"\n    },\n    \"dimensionFilters\": {\n      \"type\": \"array\"\n    },\n    \"pivoted\": {\n      \"type\": \"boolean\"\n    },\n    \"breakdown\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-report-cross-dimension-reach-criteria-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: ReportCrossDimensionReachCriteria
---
