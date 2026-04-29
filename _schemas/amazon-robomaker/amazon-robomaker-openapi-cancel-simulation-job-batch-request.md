---
description: CancelSimulationJobBatchRequest schema from openapi
layout: schema
name: CancelSimulationJobBatchRequest
properties_list:
- description: ''
  name: batch
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-cancel-simulation-job-batch-request-schema.json
slug: amazon-robomaker-openapi-cancel-simulation-job-batch-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-cancel-simulation-job-batch-request-schema.json\",\n  \"title\": \"CancelSimulationJobBatchRequest\",\n  \"description\": \"CancelSimulationJobBatchRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"batch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The id of the batch to cancel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"batch\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-cancel-simulation-job-batch-request-schema.json
tags:
- AWS
- Robotics
- Simulation
title: CancelSimulationJobBatchRequest
---
