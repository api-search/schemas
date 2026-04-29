---
description: DescribeSimulationJobRequest schema from openapi
layout: schema
name: DescribeSimulationJobRequest
properties_list:
- description: ''
  name: job
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-simulation-job-request-schema.json
slug: amazon-robomaker-openapi-describe-simulation-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-simulation-job-request-schema.json\",\n  \"title\": \"DescribeSimulationJobRequest\",\n  \"description\": \"DescribeSimulationJobRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the simulation job to be described.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"job\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-simulation-job-request-schema.json
tags:
- AWS
- Robotics
- Simulation
title: DescribeSimulationJobRequest
---
