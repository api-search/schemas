---
description: StartImagePipelineExecutionRequest schema from EC2 Image Builder
layout: schema
name: StartImagePipelineExecutionRequest
properties_list:
- description: ''
  name: imagePipelineArn
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-start-image-pipeline-execution-request-schema.json
slug: ec2-image-builder-start-image-pipeline-execution-request
source_filename: ec2-image-builder-start-image-pipeline-execution-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-start-image-pipeline-execution-request-schema.json\",\n  \"title\": \"StartImagePipelineExecutionRequest\",\n  \"description\": \"StartImagePipelineExecutionRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imagePipelineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImagePipelineArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image pipeline that you want to manually invoke.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token used to make this request idempotent.\"\n        }\n      ]\n\
  \    }\n  },\n  \"required\": [\n    \"imagePipelineArn\",\n    \"clientToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-start-image-pipeline-execution-request-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: StartImagePipelineExecutionRequest
---
