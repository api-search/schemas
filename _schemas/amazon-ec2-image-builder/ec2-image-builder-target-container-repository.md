---
description: The container repository where the output container image is stored.
layout: schema
name: TargetContainerRepository
properties_list:
- description: ''
  name: service
  type: object
- description: ''
  name: repositoryName
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-target-container-repository-schema.json
slug: ec2-image-builder-target-container-repository
source_filename: ec2-image-builder-target-container-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-target-container-repository-schema.json\",\n  \"title\": \"TargetContainerRepository\",\n  \"description\": \"The container repository where the output container image is stored.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerRepositoryService\"\n        },\n        {\n          \"description\": \"Specifies the service in which this image was registered.\"\n        }\n      ]\n    },\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the container repository where the output container image is stored. This name is prefixed by the repository\
  \ location.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"service\",\n    \"repositoryName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-target-container-repository-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: TargetContainerRepository
---
