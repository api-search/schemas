---
description: Information about a world export job.
layout: schema
name: WorldExportJobSummary
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: worlds
  type: object
- description: ''
  name: outputLocation
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-world-export-job-summary-schema.json
slug: amazon-robomaker-openapi-world-export-job-summary
source_filename: amazon-robomaker-openapi-world-export-job-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-world-export-job-summary-schema.json\",\n  \"title\": \"WorldExportJobSummary\",\n  \"description\": \"Information about a world export job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the world export job.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldExportJobStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the world export job.</p> <dl> <dt>Pending</dt> <dd> <p>The world export job request is pending.</p> </dd> <dt>Running</dt> <dd> <p>The world export job is running. </p> </dd>\
  \ <dt>Completed</dt> <dd> <p>The world export job completed. </p> </dd> <dt>Failed</dt> <dd> <p>The world export job failed. See <code>failureCode</code> for more information. </p> </dd> <dt>Canceled</dt> <dd> <p>The world export job was cancelled.</p> </dd> <dt>Canceling</dt> <dd> <p>The world export job is being cancelled.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the world export job was created.\"\n        }\n      ]\n    },\n    \"worlds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arns\"\n        },\n        {\n          \"description\": \"A list of worlds.\"\n        }\n      ]\n    },\n    \"outputLocation\": {\n      \"$ref\": \"#/components/schemas/OutputLocation\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-world-export-job-summary-schema.json
tags:
- AWS
- Robotics
- Simulation
title: WorldExportJobSummary
---
