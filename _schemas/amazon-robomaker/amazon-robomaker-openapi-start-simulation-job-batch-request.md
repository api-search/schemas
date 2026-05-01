---
description: StartSimulationJobBatchRequest schema from openapi
layout: schema
name: StartSimulationJobBatchRequest
properties_list:
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: batchPolicy
  type: object
- description: ''
  name: createSimulationJobRequests
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-start-simulation-job-batch-request-schema.json
slug: amazon-robomaker-openapi-start-simulation-job-batch-request
source_filename: amazon-robomaker-openapi-start-simulation-job-batch-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-start-simulation-job-batch-request-schema.json\",\n  \"title\": \"StartSimulationJobBatchRequest\",\n  \"description\": \"StartSimulationJobBatchRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"batchPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchPolicy\"\n        },\n        {\n          \"description\": \"The batch policy.\"\n        }\n      ]\n    },\n    \"createSimulationJobRequests\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateSimulationJobRequests\"\n        },\n        {\n          \"description\": \"A list of simulation job requests to create in the batch.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the deployment job batch.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"createSimulationJobRequests\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-start-simulation-job-batch-request-schema.json
tags:
- Robotics
- Simulation
title: StartSimulationJobBatchRequest
---
