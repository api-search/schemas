---
description: Settings that Image Builder uses to configure the ECR repository and the output container images that Amazon Inspector scans.
layout: schema
name: EcrConfiguration
properties_list:
- description: ''
  name: repositoryName
  type: object
- description: ''
  name: containerTags
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-ecr-configuration-schema.json
slug: ec2-image-builder-ecr-configuration
source_filename: ec2-image-builder-ecr-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-ecr-configuration-schema.json\",\n  \"title\": \"EcrConfiguration\",\n  \"description\": \"Settings that Image Builder uses to configure the ECR repository and the output container images that Amazon Inspector scans.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the container repository that Amazon Inspector scans to identify findings for your container images. The name includes the path for the repository location. If you don\\u2019t provide this information, Image Builder creates a repository in your account named <code>image-builder-image-scanning-repository</code> for vulnerability scans\
  \ of your output container images.\"\n        }\n      ]\n    },\n    \"containerTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"Tags for Image Builder to apply to the output container image that &amp;INS; scans. Tags can help you identify and manage your scanned images.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-ecr-configuration-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: EcrConfiguration
---
