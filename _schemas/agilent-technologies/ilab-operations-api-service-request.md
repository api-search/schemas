---
description: A service request submitted to a core facility.
layout: schema
name: Service Request
properties_list:
- description: Unique identifier for the service request.
  name: id
  type: integer
- description: Identifier of the service being requested.
  name: service_id
  type: integer
- description: Identifier of the research project to bill.
  name: project_id
  type: integer
- description: Current status of the service request.
  name: status
  type: string
- description: Number of units requested.
  name: quantity
  type: integer
- description: Additional notes or instructions for the core.
  name: notes
  type: string
- description: Timestamp when the request was submitted.
  name: submitted_at
  type: string
- description: Name of the principal investigator.
  name: principal_investigator
  type: string
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-service-request-schema.json
slug: ilab-operations-api-service-request
source_filename: ilab-operations-api-service-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-service-request-schema.json\",\n  \"title\": \"Service Request\",\n  \"description\": \"A service request submitted to a core facility.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the service request.\",\n      \"example\": 100123\n    },\n    \"service_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Identifier of the service being requested.\",\n      \"example\": 493801\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Identifier of the research project to bill.\",\n      \"example\": 987\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the service request.\",\n      \"enum\":\
  \ [\n        \"submitted\",\n        \"processing\",\n        \"completed\",\n        \"cancelled\"\n      ],\n      \"example\": \"submitted\"\n    },\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of units requested.\",\n      \"example\": 5\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Additional notes or instructions for the core.\",\n      \"example\": \"RNA sequencing for experiment batch 12\"\n    },\n    \"submitted_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the request was submitted.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"principal_investigator\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the principal investigator.\",\n      \"example\": \"Jane Smith\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-service-request-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Service Request
---
