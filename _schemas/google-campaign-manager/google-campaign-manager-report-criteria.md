---
description: Configuration for a STANDARD report type.
layout: schema
name: ReportCriteria
properties_list:
- description: The list of standard dimensions the report should include.
  name: dimensions
  type: array
- description: The list of names of metrics the report should include.
  name: metricNames
  type: array
- description: The list of filters on which dimensions are filtered.
  name: dimensionFilters
  type: array
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-report-criteria-schema.json
slug: google-campaign-manager-report-criteria
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportCriteria\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for a STANDARD report type.\",\n  \"properties\": {\n    \"dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The list of standard dimensions the report should include.\"\n    },\n    \"metricNames\": {\n      \"type\": \"array\",\n      \"description\": \"The list of names of metrics the report should include.\"\n    },\n    \"dimensionFilters\": {\n      \"type\": \"array\",\n      \"description\": \"The list of filters on which dimensions are filtered.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-report-criteria-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: ReportCriteria
---
