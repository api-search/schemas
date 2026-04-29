---
description: Information about a world generator job.
layout: schema
name: WorldGenerationJobSummary
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: template
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: worldCount
  type: object
- description: ''
  name: succeededWorldCount
  type: object
- description: ''
  name: failedWorldCount
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-world-generation-job-summary-schema.json
slug: amazon-robomaker-openapi-world-generation-job-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-world-generation-job-summary-schema.json\",\n  \"title\": \"WorldGenerationJobSummary\",\n  \"description\": \"Information about a world generator job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the world generator job.\"\n        }\n      ]\n    },\n    \"template\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of the world template.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\
  \n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the world generator job was created.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldGenerationJobStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the world generator job:</p> <dl> <dt>Pending</dt> <dd> <p>The world generator job request is pending.</p> </dd> <dt>Running</dt> <dd> <p>The world generator job is running. </p> </dd> <dt>Completed</dt> <dd> <p>The world generator job completed. </p> </dd> <dt>Failed</dt> <dd> <p>The world generator job failed. See <code>failureCode</code> for more information. </p> </dd> <dt>PartialFailed</dt> <dd> <p>Some worlds did not generate.</p> </dd> <dt>Canceled</dt> <dd> <p>The world generator job was cancelled.</p> </dd> <dt>Canceling</dt> <dd> <p>The world generator job is being cancelled.</p> </dd> </dl>\"\n        }\n      ]\n    },\n\
  \    \"worldCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldCount\"\n        },\n        {\n          \"description\": \"Information about the world count.\"\n        }\n      ]\n    },\n    \"succeededWorldCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of worlds that were generated.\"\n        }\n      ]\n    },\n    \"failedWorldCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of worlds that failed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-world-generation-job-summary-schema.json
tags:
- AWS
- Robotics
- Simulation
title: WorldGenerationJobSummary
---
