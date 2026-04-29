---
description: Details of an image pipeline.
layout: schema
name: ImagePipeline
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: platform
  type: object
- description: ''
  name: enhancedImageMetadataEnabled
  type: object
- description: ''
  name: imageRecipeArn
  type: object
- description: ''
  name: containerRecipeArn
  type: object
- description: ''
  name: infrastructureConfigurationArn
  type: object
- description: ''
  name: distributionConfigurationArn
  type: object
- description: ''
  name: imageTestsConfiguration
  type: object
- description: ''
  name: schedule
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: dateCreated
  type: object
- description: ''
  name: dateUpdated
  type: object
- description: ''
  name: dateLastRun
  type: object
- description: ''
  name: dateNextRun
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: imageScanningConfiguration
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-pipeline-schema.json
slug: ec2-image-builder-image-pipeline
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-pipeline-schema.json\",\n  \"title\": \"ImagePipeline\",\n  \"description\": \"Details of an image pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image pipeline.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the image pipeline.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\"\
  : \"The description of the image pipeline.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"The platform of the image pipeline.\"\n        }\n      ]\n    },\n    \"enhancedImageMetadataEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Collects additional information about the image being created, including the operating system (OS) version and package list. This information is used to enhance the overall experience of using EC2 Image Builder. Enabled by default.\"\n        }\n      ]\n    },\n    \"imageRecipeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image recipe associated with this image pipeline.\"\n\
  \        }\n      ]\n    },\n    \"containerRecipeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the container recipe that is used for this pipeline.\"\n        }\n      ]\n    },\n    \"infrastructureConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the infrastructure configuration associated with this image pipeline.\"\n        }\n      ]\n    },\n    \"distributionConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the distribution configuration associated with this image pipeline.\"\n        }\n      ]\n    },\n    \"imageTestsConfiguration\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/ImageTestsConfiguration\"\n        },\n        {\n          \"description\": \"The image tests configuration of the image pipeline.\"\n        }\n      ]\n    },\n    \"schedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Schedule\"\n        },\n        {\n          \"description\": \"The schedule of the image pipeline.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineStatus\"\n        },\n        {\n          \"description\": \"The status of the image pipeline.\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which this image pipeline was created.\"\n        }\n      ]\n    },\n    \"dateUpdated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\
  \n        },\n        {\n          \"description\": \"The date on which this image pipeline was last updated.\"\n        }\n      ]\n    },\n    \"dateLastRun\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"This is no longer supported, and does not return a value.\"\n        }\n      ]\n    },\n    \"dateNextRun\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"This is no longer supported, and does not return a value.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of this image pipeline.\"\n        }\n      ]\n    },\n    \"imageScanningConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageScanningConfiguration\"\
  \n        },\n        {\n          \"description\": \"Contains settings for vulnerability scans.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-pipeline-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImagePipeline
---
