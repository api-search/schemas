---
description: A run group.
layout: schema
name: RunGroupListItem
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
  name: maxGpus
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-run-group-list-item-schema.json
slug: healthomics-run-group-list-item
source_filename: healthomics-run-group-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-run-group-list-item-schema.json\",\n  \"title\": \"RunGroupListItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupArn\"\n        },\n        {\n          \"description\": \"The group's ARN.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupId\"\n        },\n        {\n          \"description\": \"The group's ID.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupName\"\n        },\n        {\n          \"description\": \"The group's name.\"\n        }\n      ]\n    },\n    \"maxCpus\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/RunGroupListItemMaxCpusInteger\"\n        },\n        {\n          \"description\": \"The group's maximum CPU count setting.\"\n        }\n      ]\n    },\n    \"maxRuns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupListItemMaxRunsInteger\"\n        },\n        {\n          \"description\": \"The group's maximum concurrent run setting.\"\n        }\n      ]\n    },\n    \"maxDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupListItemMaxDurationInteger\"\n        },\n        {\n          \"description\": \"The group's maximum duration setting in minutes.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupTimestamp\"\n        },\n        {\n          \"description\": \"When the group was created.\"\n        }\n      ]\n    },\n    \"maxGpus\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/RunGroupListItemMaxGpusInteger\"\n        },\n        {\n          \"description\": \" The maximum GPUs that can be used by a run group. \"\n        }\n      ]\n    }\n  },\n  \"description\": \"A run group.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-run-group-list-item-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: RunGroupListItem
---
