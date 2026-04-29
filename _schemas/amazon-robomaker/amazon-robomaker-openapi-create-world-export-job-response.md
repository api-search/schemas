---
description: CreateWorldExportJobResponse schema from openapi
layout: schema
name: CreateWorldExportJobResponse
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
  name: failureCode
  type: object
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: outputLocation
  type: object
- description: ''
  name: iamRole
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-create-world-export-job-response-schema.json
slug: amazon-robomaker-openapi-create-world-export-job-response
source_filename: amazon-robomaker-openapi-create-world-export-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-world-export-job-response-schema.json\",\n  \"title\": \"CreateWorldExportJobResponse\",\n  \"description\": \"CreateWorldExportJobResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the world export job.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldExportJobStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the world export job.</p> <dl> <dt>Pending</dt> <dd> <p>The world export job request is pending.</p> </dd> <dt>Running</dt> <dd> <p>The world export\
  \ job is running. </p> </dd> <dt>Completed</dt> <dd> <p>The world export job completed. </p> </dd> <dt>Failed</dt> <dd> <p>The world export job failed. See <code>failureCode</code> for more information. </p> </dd> <dt>Canceled</dt> <dd> <p>The world export job was cancelled.</p> </dd> <dt>Canceling</dt> <dd> <p>The world export job is being cancelled.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the world export job was created.\"\n        }\n      ]\n    },\n    \"failureCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldExportJobErrorCode\"\n        },\n        {\n          \"description\": \"<p>The failure code of the world export job if it failed:</p> <dl> <dt>InternalServiceError</dt> <dd> <p>Internal service error.</p> </dd> <dt>LimitExceeded</dt>\
  \ <dd> <p>The requested resource exceeds the maximum number allowed, or the number of concurrent stream requests exceeds the maximum number allowed. </p> </dd> <dt>ResourceNotFound</dt> <dd> <p>The specified resource could not be found. </p> </dd> <dt>RequestThrottled</dt> <dd> <p>The request was throttled.</p> </dd> <dt>InvalidInput</dt> <dd> <p>An input parameter in the request is not valid.</p> </dd> <dt>AllWorldGenerationFailed</dt> <dd> <p>All of the worlds in the world generation job failed. This can happen if your <code>worldCount</code> is greater than 50 or less than 1. </p> </dd> </dl> <p>For more information about troubleshooting WorldForge, see <a href=\\\"https://docs.aws.amazon.com/robomaker/latest/dg/troubleshooting-worldforge.html\\\">Troubleshooting Simulation WorldForge</a>. </p>\"\n        }\n      ]\n    },\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n         \
  \ \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"outputLocation\": {\n      \"$ref\": \"#/components/schemas/OutputLocation\"\n    },\n    \"iamRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRole\"\n        },\n        {\n          \"description\": \"The IAM role that the world export process uses to access the Amazon S3 bucket and put the export. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the world export job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-world-export-job-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: CreateWorldExportJobResponse
---
