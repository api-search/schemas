---
description: A filter on a dashboard that allows users to dynamically change query parameters across multiple tiles simultaneously.
layout: schema
name: DashboardFilter
properties_list:
- description: Unique identifier for this filter
  name: id
  type: string
- description: ID of the parent dashboard
  name: dashboard_id
  type: string
- description: Internal name of the filter
  name: name
  type: string
- description: Display title of the filter
  name: title
  type: string
- description: Filter input type
  name: type
  type: string
- description: LookML model name for field_filter type
  name: model
  type: string
- description: LookML explore name for field_filter type
  name: explore
  type: string
- description: LookML dimension for field_filter type
  name: dimension
  type: string
- description: Default filter value
  name: default_value
  type: string
- description: Whether multiple values can be selected
  name: allow_multiple_values
  type: boolean
- description: Whether the filter must have a value
  name: required
  type: boolean
- description: Row position of the filter in the filter bar
  name: row
  type: integer
- description: Other filters this filter listens to for cascading
  name: listens_to_filters
  type: array
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-dashboard-filter-schema.json
slug: looker-dashboard-filter
source_filename: looker-dashboard-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DashboardFilter\",\n  \"type\": \"object\",\n  \"description\": \"A filter on a dashboard that allows users to dynamically change query parameters across multiple tiles simultaneously.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this filter\"\n    },\n    \"dashboard_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the parent dashboard\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name of the filter\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display title of the filter\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Filter input type\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"LookML model name for field_filter type\"\n    },\n    \"explore\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"LookML explore name for field_filter type\"\n    },\n    \"dimension\": {\n      \"type\": \"string\",\n      \"description\": \"LookML dimension for field_filter type\"\n    },\n    \"default_value\": {\n      \"type\": \"string\",\n      \"description\": \"Default filter value\"\n    },\n    \"allow_multiple_values\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether multiple values can be selected\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the filter must have a value\"\n    },\n    \"row\": {\n      \"type\": \"integer\",\n      \"description\": \"Row position of the filter in the filter bar\"\n    },\n    \"listens_to_filters\": {\n      \"type\": \"array\",\n      \"description\": \"Other filters this filter listens to for cascading\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-dashboard-filter-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: DashboardFilter
---
