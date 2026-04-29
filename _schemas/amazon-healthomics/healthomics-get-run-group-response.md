---
description: ''
layout: schema
name: GetRunGroupResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: id
  type: object
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
  name: creationTime
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: maxGpus
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-get-run-group-response-schema.json
slug: healthomics-get-run-group-response
source_filename: healthomics-get-run-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-run-group-response-schema.json\",\n  \"title\": \"GetRunGroupResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupArn\"\n        },\n        {\n          \"description\": \"The group's ARN.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupId\"\n        },\n        {\n          \"description\": \"The group's ID.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupName\"\n        },\n        {\n          \"description\": \"The group's name.\"\n        }\n      ]\n    },\n    \"maxCpus\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/GetRunGroupResponseMaxCpusInteger\"\n        },\n        {\n          \"description\": \"The group's maximum number of CPUs to use.\"\n        }\n      ]\n    },\n    \"maxRuns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetRunGroupResponseMaxRunsInteger\"\n        },\n        {\n          \"description\": \"The maximum number of concurrent runs for the group.\"\n        }\n      ]\n    },\n    \"maxDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetRunGroupResponseMaxDurationInteger\"\n        },\n        {\n          \"description\": \"The group's maximum run time in minutes.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupTimestamp\"\n        },\n        {\n          \"description\": \"When the group was created.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The group's tags.\"\n        }\n      ]\n    },\n    \"maxGpus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetRunGroupResponseMaxGpusInteger\"\n        },\n        {\n          \"description\": \" The maximum GPUs that can be used by a run group. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-run-group-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: GetRunGroupResponse
---
