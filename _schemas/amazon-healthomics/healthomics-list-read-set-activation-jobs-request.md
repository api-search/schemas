---
description: ''
layout: schema
name: ListReadSetActivationJobsRequest
properties_list:
- description: ''
  name: filter
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-read-set-activation-jobs-request-schema.json
slug: healthomics-list-read-set-activation-jobs-request
source_filename: healthomics-list-read-set-activation-jobs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-read-set-activation-jobs-request-schema.json\",\n  \"title\": \"ListReadSetActivationJobsRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivateReadSetFilter\"\n        },\n        {\n          \"description\": \"A filter to apply to the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-read-set-activation-jobs-request-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListReadSetActivationJobsRequest
---
