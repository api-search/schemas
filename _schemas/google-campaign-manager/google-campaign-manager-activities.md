---
description: Represents an activity group for report filtering.
layout: schema
name: Activities
properties_list:
- description: List of activity filters.
  name: filters
  type: array
- description: List of activity metric names.
  name: metricNames
  type: array
- description: ''
  name: kind
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-activities-schema.json
slug: google-campaign-manager-activities
source_filename: google-campaign-manager-activities-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Activities\",\n  \"type\": \"object\",\n  \"description\": \"Represents an activity group for report filtering.\",\n  \"properties\": {\n    \"filters\": {\n      \"type\": \"array\",\n      \"description\": \"List of activity filters.\"\n    },\n    \"metricNames\": {\n      \"type\": \"array\",\n      \"description\": \"List of activity metric names.\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-activities-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: Activities
---
