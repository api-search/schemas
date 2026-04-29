---
description: Configuration for a REACH report type.
layout: schema
name: ReportReachCriteria
properties_list:
- description: ''
  name: dimensions
  type: array
- description: ''
  name: metricNames
  type: array
- description: ''
  name: reachByFrequencyMetricNames
  type: array
- description: ''
  name: dimensionFilters
  type: array
- description: ''
  name: enableAllDimensionCombinations
  type: boolean
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-report-reach-criteria-schema.json
slug: google-campaign-manager-report-reach-criteria
source_filename: google-campaign-manager-report-reach-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportReachCriteria\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for a REACH report type.\",\n  \"properties\": {\n    \"dimensions\": {\n      \"type\": \"array\"\n    },\n    \"metricNames\": {\n      \"type\": \"array\"\n    },\n    \"reachByFrequencyMetricNames\": {\n      \"type\": \"array\"\n    },\n    \"dimensionFilters\": {\n      \"type\": \"array\"\n    },\n    \"enableAllDimensionCombinations\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-report-reach-criteria-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: ReportReachCriteria
---
