---
description: Information about worlds that failed.
layout: schema
name: FailureSummary
properties_list:
- description: ''
  name: totalFailureCount
  type: object
- description: ''
  name: failures
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-failure-summary-schema.json
slug: amazon-robomaker-openapi-failure-summary
source_filename: amazon-robomaker-openapi-failure-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-failure-summary-schema.json\",\n  \"title\": \"FailureSummary\",\n  \"description\": \"Information about worlds that failed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalFailureCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of failures.\"\n        }\n      ]\n    },\n    \"failures\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldFailures\"\n        },\n        {\n          \"description\": \"The worlds that failed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-failure-summary-schema.json
tags:
- AWS
- Robotics
- Simulation
title: FailureSummary
---
