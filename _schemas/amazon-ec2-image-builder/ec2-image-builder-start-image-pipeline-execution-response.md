---
description: StartImagePipelineExecutionResponse schema from EC2 Image Builder
layout: schema
name: StartImagePipelineExecutionResponse
properties_list:
- description: ''
  name: requestId
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: imageBuildVersionArn
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-start-image-pipeline-execution-response-schema.json
slug: ec2-image-builder-start-image-pipeline-execution-response
source_filename: ec2-image-builder-start-image-pipeline-execution-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-start-image-pipeline-execution-response-schema.json\",\n  \"title\": \"StartImagePipelineExecutionResponse\",\n  \"description\": \"StartImagePipelineExecutionResponse schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The request ID that uniquely identifies this request.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token used to make this request idempotent.\"\n        }\n      ]\n    },\n    \"imageBuildVersionArn\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image that was created by this request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-start-image-pipeline-execution-response-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: StartImagePipelineExecutionResponse
---
