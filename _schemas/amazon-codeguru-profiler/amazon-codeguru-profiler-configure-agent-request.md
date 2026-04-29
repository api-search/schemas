---
description: The structure representing the configureAgentRequest.
layout: schema
name: ConfigureAgentRequest
properties_list:
- description: ''
  name: fleetInstanceId
  type: object
- description: ''
  name: metadata
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-configure-agent-request-schema.json
slug: amazon-codeguru-profiler-configure-agent-request
source_filename: amazon-codeguru-profiler-configure-agent-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-configure-agent-request-schema.json\",\n  \"title\": \"ConfigureAgentRequest\",\n  \"description\": \"The structure representing the configureAgentRequest.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fleetInstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetInstanceId\"\n        },\n        {\n          \"description\": \" A universally unique identifier (UUID) for a profiling instance. For example, if the profiling instance is an Amazon EC2 instance, it is the instance ID. If it is an AWS Fargate container, it is the container's task ID. \"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Metadata\"\n        },\n        {\n          \"description\"\
  : \"<p> Metadata captured about the compute platform the agent is running on. It includes information about sampling and reporting. The valid fields are:</p> <ul> <li> <p> <code>COMPUTE_PLATFORM</code> - The compute platform on which the agent is running </p> </li> <li> <p> <code>AGENT_ID</code> - The ID for an agent instance. </p> </li> <li> <p> <code>AWS_REQUEST_ID</code> - The AWS request ID of a Lambda invocation. </p> </li> <li> <p> <code>EXECUTION_ENVIRONMENT</code> - The execution environment a Lambda function is running on. </p> </li> <li> <p> <code>LAMBDA_FUNCTION_ARN</code> - The Amazon Resource Name (ARN) that is used to invoke a Lambda function. </p> </li> <li> <p> <code>LAMBDA_MEMORY_LIMIT_IN_MB</code> - The memory allocated to a Lambda function. </p> </li> <li> <p> <code>LAMBDA_REMAINING_TIME_IN_MILLISECONDS</code> - The time in milliseconds before execution of a Lambda function times out. </p> </li> <li> <p> <code>LAMBDA_TIME_GAP_BETWEEN_INVOKES_IN_MILLISECONDS</code> -\
  \ The time in milliseconds between two invocations of a Lambda function. </p> </li> <li> <p> <code>LAMBDA_PREVIOUS_EXECUTION_TIME_IN_MILLISECONDS</code> - The time in milliseconds for the previous Lambda invocation. </p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-configure-agent-request-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: ConfigureAgentRequest
---
