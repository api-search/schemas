---
description: BatchDescribeSimulationJobRequest schema from openapi
layout: schema
name: BatchDescribeSimulationJobRequest
properties_list:
- description: ''
  name: jobs
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-batch-describe-simulation-job-request-schema.json
slug: amazon-robomaker-openapi-batch-describe-simulation-job-request
source_filename: amazon-robomaker-openapi-batch-describe-simulation-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-batch-describe-simulation-job-request-schema.json\",\n  \"title\": \"BatchDescribeSimulationJobRequest\",\n  \"description\": \"BatchDescribeSimulationJobRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arns\"\n        },\n        {\n          \"description\": \"A list of Amazon Resource Names (ARNs) of simulation jobs to describe.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-batch-describe-simulation-job-request-schema.json
tags:
- Robotics
- Simulation
title: BatchDescribeSimulationJobRequest
---
