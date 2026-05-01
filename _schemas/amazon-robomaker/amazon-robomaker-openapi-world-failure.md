---
description: Information about a failed world.
layout: schema
name: WorldFailure
properties_list:
- description: ''
  name: failureCode
  type: object
- description: ''
  name: sampleFailureReason
  type: object
- description: ''
  name: failureCount
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-world-failure-schema.json
slug: amazon-robomaker-openapi-world-failure
source_filename: amazon-robomaker-openapi-world-failure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-world-failure-schema.json\",\n  \"title\": \"WorldFailure\",\n  \"description\": \"Information about a failed world.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"failureCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldGenerationJobErrorCode\"\n        },\n        {\n          \"description\": \"<p>The failure code of the world export job if it failed:</p> <dl> <dt>InternalServiceError</dt> <dd> <p>Internal service error.</p> </dd> <dt>LimitExceeded</dt> <dd> <p>The requested resource exceeds the maximum number allowed, or the number of concurrent stream requests exceeds the maximum number allowed. </p> </dd> <dt>ResourceNotFound</dt> <dd> <p>The specified resource could not be found. </p> </dd> <dt>RequestThrottled</dt> <dd>\
  \ <p>The request was throttled.</p> </dd> <dt>InvalidInput</dt> <dd> <p>An input parameter in the request is not valid.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"sampleFailureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The sample reason why the world failed. World errors are aggregated. A sample is used as the <code>sampleFailureReason</code>. \"\n        }\n      ]\n    },\n    \"failureCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of failed worlds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-world-failure-schema.json
tags:
- Robotics
- Simulation
title: WorldFailure
---
