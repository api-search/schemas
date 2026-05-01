---
description: BatchDescribeSimulationJobResponse schema from openapi
layout: schema
name: BatchDescribeSimulationJobResponse
properties_list:
- description: ''
  name: jobs
  type: object
- description: ''
  name: unprocessedJobs
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-batch-describe-simulation-job-response-schema.json
slug: amazon-robomaker-openapi-batch-describe-simulation-job-response
source_filename: amazon-robomaker-openapi-batch-describe-simulation-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-batch-describe-simulation-job-response-schema.json\",\n  \"title\": \"BatchDescribeSimulationJobResponse\",\n  \"description\": \"BatchDescribeSimulationJobResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationJobs\"\n        },\n        {\n          \"description\": \"A list of simulation jobs.\"\n        }\n      ]\n    },\n    \"unprocessedJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arns\"\n        },\n        {\n          \"description\": \"A list of unprocessed simulation job Amazon Resource Names (ARNs).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-batch-describe-simulation-job-response-schema.json
tags:
- Robotics
- Simulation
title: BatchDescribeSimulationJobResponse
---
