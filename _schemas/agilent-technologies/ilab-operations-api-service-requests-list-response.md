---
description: List of service requests for a core facility.
layout: schema
name: Service Requests List Response
properties_list:
- description: ''
  name: service_requests
  type: array
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-service-requests-list-response-schema.json
slug: ilab-operations-api-service-requests-list-response
source_filename: ilab-operations-api-service-requests-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-service-requests-list-response-schema.json\",\n  \"title\": \"Service Requests List Response\",\n  \"description\": \"List of service requests for a core facility.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service_requests\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ServiceRequest\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-service-requests-list-response-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Service Requests List Response
---
