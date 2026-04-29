---
description: A source for a read set activation job.
layout: schema
name: StartReadSetActivationJobSourceItem
properties_list:
- description: ''
  name: readSetId
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-start-read-set-activation-job-source-item-schema.json
slug: healthomics-start-read-set-activation-job-source-item
source_filename: healthomics-start-read-set-activation-job-source-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-read-set-activation-job-source-item-schema.json\",\n  \"title\": \"StartReadSetActivationJobSourceItem\",\n  \"type\": \"object\",\n  \"required\": [\n    \"readSetId\"\n  ],\n  \"properties\": {\n    \"readSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetId\"\n        },\n        {\n          \"description\": \"The source's read set ID.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A source for a read set activation job.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-read-set-activation-job-source-item-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: StartReadSetActivationJobSourceItem
---
