---
description: A research project or cost account.
layout: schema
name: Project
properties_list:
- description: Unique identifier for the project.
  name: id
  type: integer
- description: Name of the research project.
  name: name
  type: string
- description: Name of the principal investigator.
  name: pi_name
  type: string
- description: Financial account number for billing.
  name: account_number
  type: string
- description: Project status.
  name: status
  type: string
provider_name: agilent-technologies
provider_slug: agilent-technologies
schema_file: json-schema/ilab-operations-api-project-schema.json
slug: ilab-operations-api-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-project-schema.json\",\n  \"title\": \"Project\",\n  \"description\": \"A research project or cost account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the project.\",\n      \"example\": 987\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the research project.\",\n      \"example\": \"Cancer Genomics Study 2026\"\n    },\n    \"pi_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the principal investigator.\",\n      \"example\": \"Jane Smith\"\n    },\n    \"account_number\": {\n      \"type\": \"string\",\n      \"description\": \"Financial account number for billing.\",\n      \"example\": \"1234-5678\"\n    },\n  \
  \  \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Project status.\",\n      \"enum\": [\n        \"active\",\n        \"closed\"\n      ],\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agilent-technologies/refs/heads/main/json-schema/ilab-operations-api-project-schema.json
tags:
- Life Sciences
- Diagnostics
- Laboratory
- Scientific Instruments
- LIMS
- Laboratory Automation
title: Project
---
