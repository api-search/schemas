---
description: DescribeSimulationJobBatchResponse schema from openapi
layout: schema
name: DescribeSimulationJobBatchResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: batchPolicy
  type: object
- description: ''
  name: failureCode
  type: object
- description: ''
  name: failureReason
  type: object
- description: ''
  name: failedRequests
  type: object
- description: ''
  name: pendingRequests
  type: object
- description: ''
  name: createdRequests
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-simulation-job-batch-response-schema.json
slug: amazon-robomaker-openapi-describe-simulation-job-batch-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-simulation-job-batch-response-schema.json\",\n  \"title\": \"DescribeSimulationJobBatchResponse\",\n  \"description\": \"DescribeSimulationJobBatchResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the batch.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationJobBatchStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the batch.</p> <dl> <dt>Pending</dt> <dd> <p>The simulation job batch request is pending.</p> </dd> <dt>InProgress</dt> <dd> <p>The simulation\
  \ job batch is in progress. </p> </dd> <dt>Failed</dt> <dd> <p>The simulation job batch failed. One or more simulation job requests could not be completed due to an internal failure (like <code>InternalServiceError</code>). See <code>failureCode</code> and <code>failureReason</code> for more information.</p> </dd> <dt>Completed</dt> <dd> <p>The simulation batch job completed. A batch is complete when (1) there are no pending simulation job requests in the batch and none of the failed simulation job requests are due to <code>InternalServiceError</code> and (2) when all created simulation jobs have reached a terminal state (for example, <code>Completed</code> or <code>Failed</code>). </p> </dd> <dt>Canceled</dt> <dd> <p>The simulation batch job was cancelled.</p> </dd> <dt>Canceling</dt> <dd> <p>The simulation batch job is being cancelled.</p> </dd> <dt>Completing</dt> <dd> <p>The simulation batch job is completing.</p> </dd> <dt>TimingOut</dt> <dd> <p>The simulation job batch is timing\
  \ out.</p> <p>If a batch timing out, and there are pending requests that were failing due to an internal failure (like <code>InternalServiceError</code>), the batch status will be <code>Failed</code>. If there are no such failing request, the batch status will be <code>TimedOut</code>. </p> </dd> <dt>TimedOut</dt> <dd> <p>The simulation batch job timed out.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the simulation job batch was last updated.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the simulation job batch was created.\"\n        }\n      ]\n    },\n    \"clientRequestToken\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"batchPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchPolicy\"\n        },\n        {\n          \"description\": \"The batch policy.\"\n        }\n      ]\n    },\n    \"failureCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationJobBatchErrorCode\"\n        },\n        {\n          \"description\": \"The failure code of the simulation job batch.\"\n        }\n      ]\n    },\n    \"failureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The reason the simulation job batch failed.\"\n        }\n      ]\n    },\n    \"\
  failedRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedCreateSimulationJobRequests\"\n        },\n        {\n          \"description\": \"A list of failed create simulation job requests. The request failed to be created into a simulation job. Failed requests do not have a simulation job ID. \"\n        }\n      ]\n    },\n    \"pendingRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateSimulationJobRequests\"\n        },\n        {\n          \"description\": \"A list of pending simulation job requests. These requests have not yet been created into simulation jobs.\"\n        }\n      ]\n    },\n    \"createdRequests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationJobSummaries\"\n        },\n        {\n          \"description\": \"A list of created simulation job summaries.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the simulation job batch.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-simulation-job-batch-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: DescribeSimulationJobBatchResponse
---
