---
description: A core facility within an institution.
layout: schema
name: Core
properties_list:
- description: Unique identifier for the core facility.
  name: id
  type: integer
- description: Display name of the core facility.
  name: name
  type: string
- description: Name of the institution operating the core.
  name: institution
  type: string
- description: Description of the core facility's capabilities.
  name: description
  type: string
- description: Operational status of the core.
  name: status
  type: string
- description: Contact email for the core facility.
  name: contact_email
  type: string
- description: API URL for this core resource.
  name: url
  type: string
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-core-schema.json
slug: ilab-operations-api-core
source_filename: ilab-operations-api-core-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-core-schema.json\",\n  \"title\": \"Core\",\n  \"description\": \"A core facility within an institution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the core facility.\",\n      \"example\": 5582\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the core facility.\",\n      \"example\": \"Genomics Core Facility\"\n    },\n    \"institution\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the institution operating the core.\",\n      \"example\": \"Stanford University\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the core facility's capabilities.\",\n      \"example\"\
  : \"High-throughput genomics and sequencing services\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Operational status of the core.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ],\n      \"example\": \"active\"\n    },\n    \"contact_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Contact email for the core facility.\",\n      \"example\": \"genomics-core@stanford.edu\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for this core resource.\",\n      \"example\": \"https://api.ilabsolutions.com/v1/cores/5582\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-core-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Core
---
