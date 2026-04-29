---
description: A service offered by a core facility.
layout: schema
name: Service
properties_list:
- description: Unique identifier for the service.
  name: id
  type: integer
- description: Name of the service.
  name: name
  type: string
- description: Description of the service.
  name: description
  type: string
- description: Availability status of the service.
  name: status
  type: string
- description: API URL for this service resource.
  name: url
  type: string
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-service-schema.json
slug: ilab-operations-api-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-service-schema.json\",\n  \"title\": \"Service\",\n  \"description\": \"A service offered by a core facility.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the service.\",\n      \"example\": 493801\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the service.\",\n      \"example\": \"RNA Sequencing\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the service.\",\n      \"example\": \"Transcriptome sequencing service\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Availability status of the service.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\
  \n      ],\n      \"example\": \"active\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for this service resource.\",\n      \"example\": \"https://api.ilabsolutions.com/v1/cores/5582/services/493801\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-service-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Service
---
