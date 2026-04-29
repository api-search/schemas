---
description: CreateContainerRecipeRequest schema from EC2 Image Builder
layout: schema
name: CreateContainerRecipeRequest
properties_list:
- description: ''
  name: containerType
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: semanticVersion
  type: object
- description: ''
  name: components
  type: object
- description: ''
  name: instanceConfiguration
  type: object
- description: ''
  name: dockerfileTemplateData
  type: object
- description: ''
  name: dockerfileTemplateUri
  type: object
- description: ''
  name: platformOverride
  type: object
- description: ''
  name: imageOsVersionOverride
  type: object
- description: ''
  name: parentImage
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: workingDirectory
  type: object
- description: ''
  name: targetRepository
  type: object
- description: ''
  name: kmsKeyId
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-create-container-recipe-request-schema.json
slug: ec2-image-builder-create-container-recipe-request
source_filename: ec2-image-builder-create-container-recipe-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-container-recipe-request-schema.json\",\n  \"title\": \"CreateContainerRecipeRequest\",\n  \"description\": \"CreateContainerRecipeRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"containerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerType\"\n        },\n        {\n          \"description\": \"The type of container to create.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the container recipe.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\
  \n        },\n        {\n          \"description\": \"The description of the container recipe.\"\n        }\n      ]\n    },\n    \"semanticVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionNumber\"\n        },\n        {\n          \"description\": \"<p>The semantic version of the container recipe. This version follows the semantic version syntax.</p> <note> <p>The semantic version has four nodes: &lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;/&lt;build&gt;. You can assign values for the first three, and can filter on all of them.</p> <p> <b>Assignment:</b> For the first three nodes you can assign any positive integer value, including zero, with an upper limit of 2^30-1, or 1073741823 for each node. Image Builder automatically assigns the build number to the fourth node.</p> <p> <b>Patterns:</b> You can use any numeric pattern that adheres to the assignment requirements for the nodes that you can assign. For example, you might choose a software\
  \ version pattern, such as 1.0.0, or a date, such as 2021.01.01.</p> </note>\"\n        }\n      ]\n    },\n    \"components\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentConfigurationList\"\n        },\n        {\n          \"description\": \"Components for build and test that are included in the container recipe. Recipes require a minimum of one build component, and can have a maximum of 20 build and test components in any combination.\"\n        }\n      ]\n    },\n    \"instanceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceConfiguration\"\n        },\n        {\n          \"description\": \"A group of options that can be used to configure an instance for building and testing container images.\"\n        }\n      ]\n    },\n    \"dockerfileTemplateData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InlineDockerFileTemplate\"\n        },\n        {\n   \
  \       \"description\": \"The Dockerfile template used to build your image as an inline data blob.\"\n        }\n      ]\n    },\n    \"dockerfileTemplateUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uri\"\n        },\n        {\n          \"description\": \"The Amazon S3 URI for the Dockerfile that will be used to build your container image.\"\n        }\n      ]\n    },\n    \"platformOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"Specifies the operating system platform when you use a custom base image.\"\n        }\n      ]\n    },\n    \"imageOsVersionOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Specifies the operating system version for the base image.\"\n        }\n      ]\n    },\n    \"parentImage\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The base image for the container recipe.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags that are attached to the container recipe.\"\n        }\n      ]\n    },\n    \"workingDirectory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The working directory for use during build and test workflows.\"\n        }\n      ]\n    },\n    \"targetRepository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetContainerRepository\"\n        },\n        {\n          \"description\": \"The destination repository for the container image.\"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Identifies which KMS key is used to encrypt the container image.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The client token used to make this request idempotent.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"containerType\",\n    \"name\",\n    \"semanticVersion\",\n    \"components\",\n    \"parentImage\",\n    \"targetRepository\",\n    \"clientToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-container-recipe-request-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: CreateContainerRecipeRequest
---
