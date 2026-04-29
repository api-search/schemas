---
description: ''
layout: schema
name: RunStatus
properties_list: []
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-run-status-schema.json
slug: healthomics-run-status
source_filename: healthomics-run-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-run-status-schema.json\",\n  \"title\": \"RunStatus\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PENDING\",\n    \"STARTING\",\n    \"RUNNING\",\n    \"STOPPING\",\n    \"COMPLETED\",\n    \"DELETED\",\n    \"CANCELLED\",\n    \"FAILED\"\n  ],\n  \"minLength\": 1,\n  \"maxLength\": 64\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-run-status-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: RunStatus
---
