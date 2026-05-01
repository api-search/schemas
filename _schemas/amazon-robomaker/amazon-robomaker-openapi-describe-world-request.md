---
description: DescribeWorldRequest schema from openapi
layout: schema
name: DescribeWorldRequest
properties_list:
- description: ''
  name: world
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-world-request-schema.json
slug: amazon-robomaker-openapi-describe-world-request
source_filename: amazon-robomaker-openapi-describe-world-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-world-request-schema.json\",\n  \"title\": \"DescribeWorldRequest\",\n  \"description\": \"DescribeWorldRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"world\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of the world you want to describe.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"world\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-world-request-schema.json
tags:
- Robotics
- Simulation
title: DescribeWorldRequest
---
