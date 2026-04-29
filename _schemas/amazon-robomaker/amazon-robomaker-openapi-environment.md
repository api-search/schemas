---
description: The object that contains the Docker image URI for either your robot or simulation applications.
layout: schema
name: Environment
properties_list:
- description: ''
  name: uri
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-environment-schema.json
slug: amazon-robomaker-openapi-environment
source_filename: amazon-robomaker-openapi-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-environment-schema.json\",\n  \"title\": \"Environment\",\n  \"description\": \"The object that contains the Docker image URI for either your robot or simulation applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryUrl\"\n        },\n        {\n          \"description\": \"The Docker image URI for either your robot or simulation applications.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-environment-schema.json
tags:
- AWS
- Robotics
- Simulation
title: Environment
---
