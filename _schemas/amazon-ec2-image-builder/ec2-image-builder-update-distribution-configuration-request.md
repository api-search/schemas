---
description: UpdateDistributionConfigurationRequest schema from EC2 Image Builder
layout: schema
name: UpdateDistributionConfigurationRequest
properties_list:
- description: ''
  name: distributionConfigurationArn
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: distributions
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-update-distribution-configuration-request-schema.json
slug: ec2-image-builder-update-distribution-configuration-request
source_filename: ec2-image-builder-update-distribution-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-update-distribution-configuration-request-schema.json\",\n  \"title\": \"UpdateDistributionConfigurationRequest\",\n  \"description\": \"UpdateDistributionConfigurationRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"distributionConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DistributionConfigurationArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the distribution configuration that you want to update.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the distribution configuration.\"\
  \n        }\n      ]\n    },\n    \"distributions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DistributionList\"\n        },\n        {\n          \"description\": \"The distributions of the distribution configuration.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token of the distribution configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"distributionConfigurationArn\",\n    \"distributions\",\n    \"clientToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-update-distribution-configuration-request-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: UpdateDistributionConfigurationRequest
---
