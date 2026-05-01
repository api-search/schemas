---
description: A container recipe.
layout: schema
name: ContainerRecipe
properties_list:
- description: ''
  name: arn
  type: object
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
  name: instanceConfiguration
  type: object
- description: ''
  name: dockerfileTemplateData
  type: object
- description: ''
  name: kmsKeyId
  type: object
- description: ''
  name: encrypted
  type: object
- description: ''
  name: parentImage
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
  name: targetRepository
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-container-recipe-schema.json
slug: ec2-image-builder-container-recipe
source_filename: ec2-image-builder-container-recipe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-container-recipe-schema.json\",\n  \"title\": \"ContainerRecipe\",\n  \"description\": \"A container recipe.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the container recipe.</p> <note> <p>Semantic versioning is included in each object's Amazon Resource Name (ARN), at the level that applies to that object as follows:</p> <ol> <li> <p>Versionless ARNs and Name ARNs do not include specific values in any of the nodes. The nodes are either left off entirely, or they are specified as wildcards, for example: x.x.x.</p> </li> <li> <p>Version ARNs have only the first three nodes: &lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</p>\
  \ </li> <li> <p>Build version ARNs have all four nodes, and point to a specific build for a specific version of an object.</p> </li> </ol> </note>\"\n        }\n      ]\n    },\n    \"containerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerType\"\n        },\n        {\n          \"description\": \"Specifies the type of container, such as Docker.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the container recipe.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the container recipe.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n \
  \       },\n        {\n          \"description\": \"The system platform for the container, such as Windows or Linux.\"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The owner of the container recipe.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionNumber\"\n        },\n        {\n          \"description\": \"<p>The semantic version of the container recipe.</p> <note> <p>The semantic version has four nodes: &lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;/&lt;build&gt;. You can assign values for the first three, and can filter on all of them.</p> <p> <b>Assignment:</b> For the first three nodes you can assign any positive integer value, including zero, with an upper limit of 2^30-1, or 1073741823 for each node. Image Builder automatically assigns the build number to the\
  \ fourth node.</p> <p> <b>Patterns:</b> You can use any numeric pattern that adheres to the assignment requirements for the nodes that you can assign. For example, you might choose a software version pattern, such as 1.0.0, or a date, such as 2021.01.01.</p> <p> <b>Filtering:</b> With semantic versioning, you have the flexibility to use wildcards (x) to specify the most recent versions or nodes when selecting the base image or components for your recipe. When you use a wildcard in any node, all nodes to the right of the first wildcard must also be wildcards.</p> </note>\"\n        }\n      ]\n    },\n    \"components\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentConfigurationList\"\n        },\n        {\n          \"description\": \"Build and test components that are included in the container recipe. Recipes require a minimum of one build component, and can have a maximum of 20 build and test components in any combination.\"\n        }\n    \
  \  ]\n    },\n    \"instanceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceConfiguration\"\n        },\n        {\n          \"description\": \"A group of options that can be used to configure an instance for building and testing container images.\"\n        }\n      ]\n    },\n    \"dockerfileTemplateData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DockerFileTemplate\"\n        },\n        {\n          \"description\": \"Dockerfiles are text documents that are used to build Docker containers, and ensure that they contain all of the elements required by the application running inside. The template data consists of contextual variables where Image Builder places build information or scripts, based on your container image recipe.\"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n   \
  \       \"description\": \"Identifies which KMS key is used to encrypt the container image for distribution to the target Region.\"\n        }\n      ]\n    },\n    \"encrypted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"A flag that indicates if the target container is encrypted.\"\n        }\n      ]\n    },\n    \"parentImage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The base image for the container recipe.\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date when this container recipe was created.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\
  \n        },\n        {\n          \"description\": \"Tags that are attached to the container recipe.\"\n        }\n      ]\n    },\n    \"workingDirectory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The working directory for use during build and test workflows.\"\n        }\n      ]\n    },\n    \"targetRepository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetContainerRepository\"\n        },\n        {\n          \"description\": \"The destination repository for the container image.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-container-recipe-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ContainerRecipe
---
