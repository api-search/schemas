---
description: ''
layout: schema
name: WorkflowStatus
properties_list: []
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-workflow-status-schema.json
slug: healthomics-workflow-status
source_filename: healthomics-workflow-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-workflow-status-schema.json\",\n  \"title\": \"WorkflowStatus\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CREATING\",\n    \"ACTIVE\",\n    \"UPDATING\",\n    \"DELETED\",\n    \"FAILED\",\n    \"INACTIVE\"\n  ],\n  \"minLength\": 1,\n  \"maxLength\": 64\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-workflow-status-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: WorkflowStatus
---
