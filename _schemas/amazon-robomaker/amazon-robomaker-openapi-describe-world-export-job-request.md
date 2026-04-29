---
description: DescribeWorldExportJobRequest schema from openapi
layout: schema
name: DescribeWorldExportJobRequest
properties_list:
- description: ''
  name: job
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-world-export-job-request-schema.json
slug: amazon-robomaker-openapi-describe-world-export-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-world-export-job-request-schema.json\",\n  \"title\": \"DescribeWorldExportJobRequest\",\n  \"description\": \"DescribeWorldExportJobRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of the world export job to describe.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"job\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-world-export-job-request-schema.json
tags:
- AWS
- Robotics
- Simulation
title: DescribeWorldExportJobRequest
---
