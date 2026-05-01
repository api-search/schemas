---
description: Container distribution settings for encryption, licensing, and sharing in a specific Region.
layout: schema
name: ContainerDistributionConfiguration
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: containerTags
  type: object
- description: ''
  name: targetRepository
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-container-distribution-configuration-schema.json
slug: ec2-image-builder-container-distribution-configuration
source_filename: ec2-image-builder-container-distribution-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-container-distribution-configuration-schema.json\",\n  \"title\": \"ContainerDistributionConfiguration\",\n  \"description\": \"Container distribution settings for encryption, licensing, and sharing in a specific Region.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the container distribution configuration.\"\n        }\n      ]\n    },\n    \"containerTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"Tags that are attached to the container distribution configuration.\"\n        }\n      ]\n\
  \    },\n    \"targetRepository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetContainerRepository\"\n        },\n        {\n          \"description\": \"The destination repository for the container distribution configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"targetRepository\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-container-distribution-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ContainerDistributionConfiguration
---
