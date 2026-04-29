---
description: CreateImageRequest schema from EC2 Image Builder
layout: schema
name: CreateImageRequest
properties_list:
- description: ''
  name: imageRecipeArn
  type: object
- description: ''
  name: containerRecipeArn
  type: object
- description: ''
  name: distributionConfigurationArn
  type: object
- description: ''
  name: infrastructureConfigurationArn
  type: object
- description: ''
  name: imageTestsConfiguration
  type: object
- description: ''
  name: enhancedImageMetadataEnabled
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: imageScanningConfiguration
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-create-image-request-schema.json
slug: ec2-image-builder-create-image-request
source_filename: ec2-image-builder-create-image-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-image-request-schema.json\",\n  \"title\": \"CreateImageRequest\",\n  \"description\": \"CreateImageRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imageRecipeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageRecipeArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image recipe that defines how images are configured, tested, and assessed.\"\n        }\n      ]\n    },\n    \"containerRecipeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerRecipeArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the container recipe that defines how images are configured and\
  \ tested.\"\n        }\n      ]\n    },\n    \"distributionConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DistributionConfigurationArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the distribution configuration that defines and configures the outputs of your pipeline.\"\n        }\n      ]\n    },\n    \"infrastructureConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InfrastructureConfigurationArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the infrastructure configuration that defines the environment in which your image will be built and tested.\"\n        }\n      ]\n    },\n    \"imageTestsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageTestsConfiguration\"\n        },\n        {\n          \"description\": \"The image tests configuration of the image.\"\
  \n        }\n      ]\n    },\n    \"enhancedImageMetadataEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Collects additional information about the image being created, including the operating system (OS) version and package list. This information is used to enhance the overall experience of using EC2 Image Builder. Enabled by default.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of the image.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token used to make this request idempotent.\"\n        }\n      ]\n    },\n    \"imageScanningConfiguration\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/ImageScanningConfiguration\"\n        },\n        {\n          \"description\": \"Contains settings for vulnerability scans.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"infrastructureConfigurationArn\",\n    \"clientToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-image-request-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: CreateImageRequest
---
