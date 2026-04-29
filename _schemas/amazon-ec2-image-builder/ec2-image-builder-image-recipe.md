---
description: An image recipe.
layout: schema
name: ImageRecipe
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: type
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
  name: owner
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: components
  type: object
- description: ''
  name: parentImage
  type: object
- description: ''
  name: blockDeviceMappings
  type: object
- description: ''
  name: dateCreated
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: workingDirectory
  type: object
- description: ''
  name: additionalInstanceConfiguration
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-recipe-schema.json
slug: ec2-image-builder-image-recipe
source_filename: ec2-image-builder-image-recipe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-recipe-schema.json\",\n  \"title\": \"ImageRecipe\",\n  \"description\": \"An image recipe.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image recipe.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageType\"\n        },\n        {\n          \"description\": \"Specifies which type of image is created by the recipe - an AMI or a container image.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n \
  \       {\n          \"description\": \"The name of the image recipe.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the image recipe.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"The platform of the image recipe.\"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The owner of the image recipe.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionNumber\"\n        },\n        {\n          \"description\": \"The version of the image recipe.\"\n        }\n    \
  \  ]\n    },\n    \"components\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentConfigurationList\"\n        },\n        {\n          \"description\": \"The components that are included in the image recipe. Recipes require a minimum of one build component, and can have a maximum of 20 build and test components in any combination.\"\n        }\n      ]\n    },\n    \"parentImage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The base image of the image recipe.\"\n        }\n      ]\n    },\n    \"blockDeviceMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceBlockDeviceMappings\"\n        },\n        {\n          \"description\": \"The block device mappings to apply when creating images from this recipe.\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which this image recipe was created.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of the image recipe.\"\n        }\n      ]\n    },\n    \"workingDirectory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The working directory to be used during build and test workflows.\"\n        }\n      ]\n    },\n    \"additionalInstanceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdditionalInstanceConfiguration\"\n        },\n        {\n          \"description\": \"Before you create a new AMI, Image Builder launches temporary Amazon EC2 instances to build and test your image configuration. Instance\
  \ configuration adds a layer of control over those instances. You can define settings and add scripts to run when an instance is launched from your AMI.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-recipe-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageRecipe
---
