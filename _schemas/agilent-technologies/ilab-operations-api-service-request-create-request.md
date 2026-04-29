---
description: Request body for creating a new service request.
layout: schema
name: Service Request Create Request
properties_list:
- description: Identifier of the service to request.
  name: service_id
  type: integer
- description: Identifier of the research project to bill.
  name: project_id
  type: integer
- description: Number of units to request.
  name: quantity
  type: integer
- description: Additional notes for the core facility.
  name: notes
  type: string
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-service-request-create-request-schema.json
slug: ilab-operations-api-service-request-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-service-request-create-request-schema.json\",\n  \"title\": \"Service Request Create Request\",\n  \"description\": \"Request body for creating a new service request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Identifier of the service to request.\",\n      \"example\": 493801\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Identifier of the research project to bill.\",\n      \"example\": 987\n    },\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of units to request.\",\n      \"example\": 5\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Additional notes for the core facility.\",\n   \
  \   \"example\": \"RNA sequencing for experiment batch 12\"\n    }\n  },\n  \"required\": [\n    \"service_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-service-request-create-request-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Service Request Create Request
---
