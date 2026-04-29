---
description: CreateAnnotationRequest schema from Amplitude Chart Annotations API
layout: schema
name: CreateAnnotationRequest
properties_list:
- description: The display label for the annotation.
  name: label
  type: string
- description: The date of the annotation in YYYY-MM-DD format.
  name: date
  type: string
- description: The end date for date-range annotations in YYYY-MM-DD format.
  name: end_date
  type: string
- description: Additional details or notes for the annotation.
  name: details
  type: string
- description: The category to assign to the annotation.
  name: category
  type: string
- description: The ID of the chart to associate the annotation with. Omit for project-wide annotations.
  name: chart_id
  type: integer
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/chart-annotations-api-create-annotation-request-schema.json
slug: chart-annotations-api-create-annotation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/chart-annotations-api-create-annotation-request-schema.json\",\n  \"title\": \"CreateAnnotationRequest\",\n  \"description\": \"CreateAnnotationRequest schema from Amplitude Chart Annotations API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The display label for the annotation.\",\n      \"maxLength\": 255\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of the annotation in YYYY-MM-DD format.\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The end date for date-range annotations in YYYY-MM-DD format.\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details\
  \ or notes for the annotation.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category to assign to the annotation.\"\n    },\n    \"chart_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the chart to associate the annotation with. Omit for project-wide annotations.\"\n    }\n  },\n  \"required\": [\n    \"label\",\n    \"date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/chart-annotations-api-create-annotation-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: CreateAnnotationRequest
---
