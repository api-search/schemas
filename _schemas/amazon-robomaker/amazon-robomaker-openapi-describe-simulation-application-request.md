---
description: DescribeSimulationApplicationRequest schema from openapi
layout: schema
name: DescribeSimulationApplicationRequest
properties_list:
- description: ''
  name: application
  type: object
- description: ''
  name: applicationVersion
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-simulation-application-request-schema.json
slug: amazon-robomaker-openapi-describe-simulation-application-request
source_filename: amazon-robomaker-openapi-describe-simulation-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-simulation-application-request-schema.json\",\n  \"title\": \"DescribeSimulationApplicationRequest\",\n  \"description\": \"DescribeSimulationApplicationRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The application information for the simulation application.\"\n        }\n      ]\n    },\n    \"applicationVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the simulation application to describe.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"application\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-simulation-application-request-schema.json
tags:
- Robotics
- Simulation
title: DescribeSimulationApplicationRequest
---
