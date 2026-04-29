---
description: Information about worlds that finished.
layout: schema
name: FinishedWorldsSummary
properties_list:
- description: ''
  name: finishedCount
  type: object
- description: ''
  name: succeededWorlds
  type: object
- description: ''
  name: failureSummary
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-finished-worlds-summary-schema.json
slug: amazon-robomaker-openapi-finished-worlds-summary
source_filename: amazon-robomaker-openapi-finished-worlds-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-finished-worlds-summary-schema.json\",\n  \"title\": \"FinishedWorldsSummary\",\n  \"description\": \"Information about worlds that finished.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"finishedCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of finished worlds.\"\n        }\n      ]\n    },\n    \"succeededWorlds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arns\"\n        },\n        {\n          \"description\": \"A list of worlds that succeeded.\"\n        }\n      ]\n    },\n    \"failureSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureSummary\"\n        },\n      \
  \  {\n          \"description\": \"Information about worlds that failed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-finished-worlds-summary-schema.json
tags:
- AWS
- Robotics
- Simulation
title: FinishedWorldsSummary
---
