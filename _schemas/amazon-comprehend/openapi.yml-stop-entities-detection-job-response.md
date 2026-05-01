---
description: StopEntitiesDetectionJobResponse schema
layout: schema
name: StopEntitiesDetectionJobResponse
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobStatus
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-stop-entities-detection-job-response-schema.json
slug: openapi.yml-stop-entities-detection-job-response
source_filename: openapi.yml-stop-entities-detection-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-stop-entities-detection-job-response-schema.json\",\n  \"title\": \"StopEntitiesDetectionJobResponse\",\n  \"description\": \"StopEntitiesDetectionJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The identifier of the entities detection job to stop.\"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"Either <code>STOP_REQUESTED</code> if the job is currently running, or <code>STOPPED</code> if the job was previously stopped with the <code>StopEntitiesDetectionJob</code> operation.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-stop-entities-detection-job-response-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: StopEntitiesDetectionJobResponse
---
