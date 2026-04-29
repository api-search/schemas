---
description: Annotation schema from Amplitude Chart Annotations API
layout: schema
name: Annotation
properties_list:
- description: The unique identifier of the annotation.
  name: id
  type: integer
- description: The display label for the annotation.
  name: label
  type: string
- description: The start date of the annotation in YYYY-MM-DD format.
  name: date
  type: string
- description: The end date of the annotation for date ranges. Null for point-in-time annotations.
  name: end_date
  type: string
- description: Additional details or notes for the annotation.
  name: details
  type: string
- description: The category of the annotation for organization purposes.
  name: category
  type: string
- description: The ID of the chart the annotation is associated with. Null for project-wide annotations.
  name: chart_id
  type: integer
- description: The timestamp when the annotation was created.
  name: created_at
  type: string
- description: The timestamp when the annotation was last updated.
  name: updated_at
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/chart-annotations-api-annotation-schema.json
slug: chart-annotations-api-annotation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/chart-annotations-api-annotation-schema.json\",\n  \"title\": \"Annotation\",\n  \"description\": \"Annotation schema from Amplitude Chart Annotations API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the annotation.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The display label for the annotation.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The start date of the annotation in YYYY-MM-DD format.\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The end date of the annotation for date ranges. Null for point-in-time annotations.\"\n    },\n    \"\
  details\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details or notes for the annotation.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the annotation for organization purposes.\"\n    },\n    \"chart_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the chart the annotation is associated with. Null for project-wide annotations.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the annotation was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the annotation was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/chart-annotations-api-annotation-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: Annotation
---
