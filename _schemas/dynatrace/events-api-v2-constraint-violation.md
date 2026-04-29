---
description: Details of a single constraint violation in a request.
layout: schema
name: ConstraintViolation
properties_list:
- description: The JSON path to the field that caused the violation.
  name: path
  type: string
- description: A description of the constraint violation.
  name: message
  type: string
- description: The location of the violating parameter (QUERY, PATH, BODY).
  name: parameterLocation
  type: string
- description: The location detail for the violation.
  name: location
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/events-api-v2-constraint-violation-schema.json
slug: events-api-v2-constraint-violation
source_filename: events-api-v2-constraint-violation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/events-api-v2-constraint-violation-schema.json\",\n  \"title\": \"ConstraintViolation\",\n  \"description\": \"Details of a single constraint violation in a request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON path to the field that caused the violation.\",\n      \"example\": \"example-value\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the constraint violation.\",\n      \"example\": \"Example description.\"\n    },\n    \"parameterLocation\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the violating parameter (QUERY, PATH, BODY).\",\n      \"example\": \"example-value\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The location detail for the violation.\",\n      \"example\": \"example-value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/events-api-v2-constraint-violation-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: ConstraintViolation
---
