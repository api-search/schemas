---
description: Represents a specific warning or failure.
layout: schema
name: Problem
properties_list:
- description: ''
  name: run
  type: object
- description: ''
  name: job
  type: object
- description: ''
  name: suite
  type: object
- description: ''
  name: test
  type: object
- description: ''
  name: device
  type: object
- description: ''
  name: result
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-problem-schema.json
slug: amazon-device-farm-problem
source_filename: amazon-device-farm-problem-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-problem-schema.json\",\n  \"title\": \"Problem\",\n  \"description\": \"Represents a specific warning or failure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"run\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProblemDetail\"\n        },\n        {\n          \"description\": \"Information about the associated run.\"\n        }\n      ]\n    },\n    \"job\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProblemDetail\"\n        },\n        {\n          \"description\": \"Information about the associated job.\"\n        }\n      ]\n    },\n    \"suite\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProblemDetail\"\n        },\n        {\n          \"description\": \"Information\
  \ about the associated suite.\"\n        }\n      ]\n    },\n    \"test\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProblemDetail\"\n        },\n        {\n          \"description\": \"Information about the associated test.\"\n        }\n      ]\n    },\n    \"device\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Device\"\n        },\n        {\n          \"description\": \"Information about the associated device.\"\n        }\n      ]\n    },\n    \"result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionResult\"\n        },\n        {\n          \"description\": \"<p>The problem's result.</p> <p>Allowed values include:</p> <ul> <li> <p>PENDING</p> </li> <li> <p>PASSED</p> </li> <li> <p>WARNED</p> </li> <li> <p>FAILED</p> </li> <li> <p>SKIPPED</p> </li> <li> <p>ERRORED</p> </li> <li> <p>STOPPED</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"A message about the problem's result.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-problem-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: Problem
---
