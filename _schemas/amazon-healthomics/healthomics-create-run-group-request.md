---
description: ''
layout: schema
name: CreateRunGroupRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: maxCpus
  type: object
- description: ''
  name: maxRuns
  type: object
- description: ''
  name: maxDuration
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: requestId
  type: object
- description: ''
  name: maxGpus
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-create-run-group-request-schema.json
slug: healthomics-create-run-group-request
source_filename: healthomics-create-run-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-run-group-request-schema.json\",\n  \"title\": \"CreateRunGroupRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"requestId\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupName\"\n        },\n        {\n          \"description\": \"A name for the group.\"\n        }\n      ]\n    },\n    \"maxCpus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateRunGroupRequestMaxCpusInteger\"\n        },\n        {\n          \"description\": \"The maximum number of CPUs to use in the group.\"\n        }\n      ]\n    },\n    \"maxRuns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateRunGroupRequestMaxRunsInteger\"\n        },\n    \
  \    {\n          \"description\": \"The maximum number of concurrent runs for the group.\"\n        }\n      ]\n    },\n    \"maxDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateRunGroupRequestMaxDurationInteger\"\n        },\n        {\n          \"description\": \"A maximum run time for the group in minutes.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags for the group.\"\n        }\n      ]\n    },\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupRequestId\"\n        },\n        {\n          \"description\": \"To ensure that requests don't run multiple times, specify a unique ID for each request.\"\n        }\n      ]\n    },\n    \"maxGpus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateRunGroupRequestMaxGpusInteger\"\
  \n        },\n        {\n          \"description\": \" The maximum GPUs that can be used by a run group. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-run-group-request-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CreateRunGroupRequest
---
