---
description: ''
layout: schema
name: JobStatus
properties_list: []
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-job-status-schema.json
slug: healthlake-job-status
source_filename: healthlake-job-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-job-status-schema.json\",\n  \"title\": \"JobStatus\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SUBMITTED\",\n    \"IN_PROGRESS\",\n    \"COMPLETED_WITH_ERRORS\",\n    \"COMPLETED\",\n    \"FAILED\",\n    \"CANCEL_SUBMITTED\",\n    \"CANCEL_IN_PROGRESS\",\n    \"CANCEL_COMPLETED\",\n    \"CANCEL_FAILED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-job-status-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: JobStatus
---
