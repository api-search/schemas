---
description: DescribeWorldGenerationJobResponse schema from openapi
layout: schema
name: DescribeWorldGenerationJobResponse
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
  name: failureReason
  type: object
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: template
  type: object
- description: ''
  name: worldCount
  type: object
- description: ''
  name: finishedWorldsSummary
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: worldTags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-world-generation-job-response-schema.json
slug: amazon-robomaker-openapi-describe-world-generation-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-world-generation-job-response-schema.json\",\n  \"title\": \"DescribeWorldGenerationJobResponse\",\n  \"description\": \"DescribeWorldGenerationJobResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the world generation job.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldGenerationJobStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the world generation job:</p> <dl> <dt>Pending</dt> <dd> <p>The world generation job request is pending.</p> </dd> <dt>Running</dt>\
  \ <dd> <p>The world generation job is running. </p> </dd> <dt>Completed</dt> <dd> <p>The world generation job completed. </p> </dd> <dt>Failed</dt> <dd> <p>The world generation job failed. See <code>failureCode</code> for more information. </p> </dd> <dt>PartialFailed</dt> <dd> <p>Some worlds did not generate.</p> </dd> <dt>Canceled</dt> <dd> <p>The world generation job was cancelled.</p> </dd> <dt>Canceling</dt> <dd> <p>The world generation job is being cancelled.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the world generation job was created.\"\n        }\n      ]\n    },\n    \"failureCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldGenerationJobErrorCode\"\n        },\n        {\n          \"description\": \"<p>The failure code of the\
  \ world generation job if it failed:</p> <dl> <dt>InternalServiceError</dt> <dd> <p>Internal service error.</p> </dd> <dt>LimitExceeded</dt> <dd> <p>The requested resource exceeds the maximum number allowed, or the number of concurrent stream requests exceeds the maximum number allowed. </p> </dd> <dt>ResourceNotFound</dt> <dd> <p>The specified resource could not be found. </p> </dd> <dt>RequestThrottled</dt> <dd> <p>The request was throttled.</p> </dd> <dt>InvalidInput</dt> <dd> <p>An input parameter in the request is not valid.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"failureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The reason why the world generation job failed.\"\n        }\n      ]\n    },\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\"\
  : \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"template\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (arn) of the world template.\"\n        }\n      ]\n    },\n    \"worldCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldCount\"\n        },\n        {\n          \"description\": \"Information about the world count.\"\n        }\n      ]\n    },\n    \"finishedWorldsSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FinishedWorldsSummary\"\n        },\n        {\n          \"description\": \"Summary information about finished worlds.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\"\
  : \"A map that contains tag keys and tag values that are attached to the world generation job.\"\n        }\n      ]\n    },\n    \"worldTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the generated worlds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-world-generation-job-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: DescribeWorldGenerationJobResponse
---
