---
description: Information about a simulation job batch.
layout: schema
name: SimulationJobBatchSummary
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: failedRequestCount
  type: object
- description: ''
  name: pendingRequestCount
  type: object
- description: ''
  name: createdRequestCount
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-simulation-job-batch-summary-schema.json
slug: amazon-robomaker-openapi-simulation-job-batch-summary
source_filename: amazon-robomaker-openapi-simulation-job-batch-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-job-batch-summary-schema.json\",\n  \"title\": \"SimulationJobBatchSummary\",\n  \"description\": \"Information about a simulation job batch.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the batch.\"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the simulation job batch was last updated.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the simulation job batch was created.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationJobBatchStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the simulation job batch.</p> <dl> <dt>Pending</dt> <dd> <p>The simulation job batch request is pending.</p> </dd> <dt>InProgress</dt> <dd> <p>The simulation job batch is in progress. </p> </dd> <dt>Failed</dt> <dd> <p>The simulation job batch failed. One or more simulation job requests could not be completed due to an internal failure (like <code>InternalServiceError</code>). See <code>failureCode</code> and <code>failureReason</code> for more information.</p> </dd> <dt>Completed</dt> <dd> <p>The simulation batch job completed. A batch is complete when (1) there are no pending simulation job requests\
  \ in the batch and none of the failed simulation job requests are due to <code>InternalServiceError</code> and (2) when all created simulation jobs have reached a terminal state (for example, <code>Completed</code> or <code>Failed</code>). </p> </dd> <dt>Canceled</dt> <dd> <p>The simulation batch job was cancelled.</p> </dd> <dt>Canceling</dt> <dd> <p>The simulation batch job is being cancelled.</p> </dd> <dt>Completing</dt> <dd> <p>The simulation batch job is completing.</p> </dd> <dt>TimingOut</dt> <dd> <p>The simulation job batch is timing out.</p> <p>If a batch timing out, and there are pending requests that were failing due to an internal failure (like <code>InternalServiceError</code>), the batch status will be <code>Failed</code>. If there are no such failing request, the batch status will be <code>TimedOut</code>. </p> </dd> <dt>TimedOut</dt> <dd> <p>The simulation batch job timed out.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"failedRequestCount\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of failed simulation job requests.\"\n        }\n      ]\n    },\n    \"pendingRequestCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of pending simulation job requests.\"\n        }\n      ]\n    },\n    \"createdRequestCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of created simulation job requests.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-job-batch-summary-schema.json
tags:
- AWS
- Robotics
- Simulation
title: SimulationJobBatchSummary
---
