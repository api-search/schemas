---
description: <p>The environment variables to send to the container. You can add new environment variables, which are added to the container at launch, or you can override the existing environment variables from the Docker image or the task definition.</p> <note> <p>Environment variables cannot start with "<code>Batch</code>". This naming convention is reserved for variables that Batch sets.</p> </note>
layout: schema
name: BatchEnvironmentVariable
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-batch-environment-variable-schema.json
slug: amazon-eventbridge-pipes-batch-environment-variable
source_filename: amazon-eventbridge-pipes-batch-environment-variable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-batch-environment-variable-schema.json\",\n  \"title\": \"BatchEnvironmentVariable\",\n  \"description\": \"<p>The environment variables to send to the container. You can add new environment variables, which are added to the container at launch, or you can override the existing environment variables from the Docker image or the task definition.</p> <note> <p>Environment variables cannot start with \\\"<code>Batch</code>\\\". This naming convention is reserved for variables that Batch sets.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the key-value pair. For environment variables, this is the\
  \ name of the environment variable.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The value of the key-value pair. For environment variables, this is the value of the environment variable.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-batch-environment-variable-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: BatchEnvironmentVariable
---
