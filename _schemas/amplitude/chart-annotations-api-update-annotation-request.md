---
description: UpdateAnnotationRequest schema from Amplitude Chart Annotations API
layout: schema
name: UpdateAnnotationRequest
properties_list:
- description: The updated display label for the annotation.
  name: label
  type: string
- description: The updated date in YYYY-MM-DD format.
  name: date
  type: string
- description: The updated end date in YYYY-MM-DD format.
  name: end_date
  type: string
- description: Updated additional details or notes.
  name: details
  type: string
- description: The updated category.
  name: category
  type: string
- description: The updated chart ID.
  name: chart_id
  type: integer
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/chart-annotations-api-update-annotation-request-schema.json
slug: chart-annotations-api-update-annotation-request
source_filename: chart-annotations-api-update-annotation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/chart-annotations-api-update-annotation-request-schema.json\",\n  \"title\": \"UpdateAnnotationRequest\",\n  \"description\": \"UpdateAnnotationRequest schema from Amplitude Chart Annotations API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The updated display label for the annotation.\",\n      \"maxLength\": 255\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The updated date in YYYY-MM-DD format.\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The updated end date in YYYY-MM-DD format.\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Updated additional details or notes.\"\
  \n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The updated category.\"\n    },\n    \"chart_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The updated chart ID.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/chart-annotations-api-update-annotation-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UpdateAnnotationRequest
---
