---
description: Represents a CI/CD pipeline in JFrog Pipelines, defining automated build, test, and deployment workflows that are natively integrated with the JFrog Platform.
layout: schema
name: JFrog Pipeline
properties_list:
- description: Unique pipeline identifier
  name: id
  type: integer
- description: Pipeline name as defined in the pipeline YAML
  name: name
  type: string
- description: ID of the pipeline source containing this pipeline definition
  name: pipelineSourceId
  type: integer
- description: Project ID this pipeline belongs to
  name: projectId
  type: integer
- description: ID of the most recent pipeline run
  name: latestRunId
  type: integer
- description: ID of the most recent completed run
  name: latestCompletedRunId
  type: integer
- description: ''
  name: latestRun
  type: object
- description: Pipeline creation timestamp
  name: createdAt
  type: string
- description: Last update timestamp
  name: updatedAt
  type: string
provider_name: JFrog
provider_slug: jfrog
schema_file: json-schema/jfrog-pipeline-schema.json
slug: jfrog-pipeline
source_filename: jfrog-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/pipeline\",\n  \"title\": \"JFrog Pipeline\",\n  \"description\": \"Represents a CI/CD pipeline in JFrog Pipelines, defining automated build, test, and deployment workflows that are natively integrated with the JFrog Platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique pipeline identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Pipeline name as defined in the pipeline YAML\",\n      \"examples\": [\n        \"my_app_pipeline\",\n        \"release_pipeline\"\n      ]\n    },\n    \"pipelineSourceId\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the pipeline source containing this pipeline definition\"\n    },\n    \"projectId\": {\n      \"type\": \"integer\",\n      \"description\": \"Project ID this pipeline belongs to\"\n\
  \    },\n    \"latestRunId\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the most recent pipeline run\"\n    },\n    \"latestCompletedRunId\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the most recent completed run\"\n    },\n    \"latestRun\": {\n      \"$ref\": \"#/$defs/Run\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Pipeline creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ],\n  \"$defs\": {\n    \"Run\": {\n      \"type\": \"object\",\n      \"description\": \"A single execution of a pipeline\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"pipelineId\": {\n          \"type\": \"integer\"\n        },\n        \"statusCode\": {\n          \"type\": \"\
  integer\",\n          \"description\": \"Run status code: 4001=queued, 4002=processing, 4003=success, 4004=error, 4005=cancelled, 4006=timeout, 4007=skipped\"\n        },\n        \"runNumber\": {\n          \"type\": \"integer\"\n        },\n        \"branchName\": {\n          \"type\": \"string\"\n        },\n        \"startedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"endedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"durationSeconds\": {\n          \"type\": \"integer\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"Step\": {\n      \"type\": \"object\",\n      \"description\": \"An individual step within a pipeline run\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n\
  \        \"pipelineId\": {\n          \"type\": \"integer\"\n        },\n        \"runId\": {\n          \"type\": \"integer\"\n        },\n        \"typeCode\": {\n          \"type\": \"integer\"\n        },\n        \"statusCode\": {\n          \"type\": \"integer\"\n        },\n        \"startedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"endedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"durationSeconds\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/json-schema/jfrog-pipeline-schema.json
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
title: JFrog Pipeline
---
