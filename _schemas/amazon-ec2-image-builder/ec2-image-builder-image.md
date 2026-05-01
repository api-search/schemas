---
description: An Image Builder image. You must specify exactly one recipe for the image – either a container recipe (<code>containerRecipe</code>), which creates a container image, or an image recipe (<code>imageRecipe</code>), which creates an AMI.
layout: schema
name: Image
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
  name: version
  type: object
- description: ''
  name: platform
  type: object
- description: ''
  name: enhancedImageMetadataEnabled
  type: object
- description: ''
  name: osVersion
  type: object
- description: ''
  name: state
  type: object
- description: ''
  name: imageRecipe
  type: object
- description: ''
  name: containerRecipe
  type: object
- description: ''
  name: sourcePipelineName
  type: object
- description: ''
  name: sourcePipelineArn
  type: object
- description: ''
  name: infrastructureConfiguration
  type: object
- description: ''
  name: distributionConfiguration
  type: object
- description: ''
  name: imageTestsConfiguration
  type: object
- description: ''
  name: dateCreated
  type: object
- description: ''
  name: outputResources
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: buildType
  type: object
- description: ''
  name: imageSource
  type: object
- description: ''
  name: scanState
  type: object
- description: ''
  name: imageScanningConfiguration
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-schema.json
slug: ec2-image-builder-image
source_filename: ec2-image-builder-image-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-schema.json\",\n  \"title\": \"Image\",\n  \"description\": \"An Image Builder image. You must specify exactly one recipe for the image \\u2013 either a container recipe (<code>containerRecipe</code>), which creates a container image, or an image recipe (<code>imageRecipe</code>), which creates an AMI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the image.</p> <note> <p>Semantic versioning is included in each object's Amazon Resource Name (ARN), at the level that applies to that object as follows:</p> <ol> <li> <p>Versionless ARNs and Name ARNs do not include specific values\
  \ in any of the nodes. The nodes are either left off entirely, or they are specified as wildcards, for example: x.x.x.</p> </li> <li> <p>Version ARNs have only the first three nodes: &lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</p> </li> <li> <p>Build version ARNs have all four nodes, and point to a specific build for a specific version of an object.</p> </li> </ol> </note>\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageType\"\n        },\n        {\n          \"description\": \"Specifies whether this image produces an AMI or a container image.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the image.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionNumber\"\n        },\n    \
  \    {\n          \"description\": \"<p>The semantic version of the image.</p> <note> <p>The semantic version has four nodes: &lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;/&lt;build&gt;. You can assign values for the first three, and can filter on all of them.</p> <p> <b>Assignment:</b> For the first three nodes you can assign any positive integer value, including zero, with an upper limit of 2^30-1, or 1073741823 for each node. Image Builder automatically assigns the build number to the fourth node.</p> <p> <b>Patterns:</b> You can use any numeric pattern that adheres to the assignment requirements for the nodes that you can assign. For example, you might choose a software version pattern, such as 1.0.0, or a date, such as 2021.01.01.</p> <p> <b>Filtering:</b> With semantic versioning, you have the flexibility to use wildcards (x) to specify the most recent versions or nodes when selecting the base image or components for your recipe. When you use a wildcard in any node, all nodes to the\
  \ right of the first wildcard must also be wildcards.</p> </note>\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"The image operating system platform, such as Linux or Windows.\"\n        }\n      ]\n    },\n    \"enhancedImageMetadataEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Indicates whether Image Builder collects additional information about the image, such as the operating system (OS) version and package list.\"\n        }\n      ]\n    },\n    \"osVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OsVersion\"\n        },\n        {\n          \"description\": \"The operating system version for instances that launch from this image. For example, Amazon Linux 2, Ubuntu 18, or Microsoft Windows\
  \ Server 2019.\"\n        }\n      ]\n    },\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageState\"\n        },\n        {\n          \"description\": \"The state of the image.\"\n        }\n      ]\n    },\n    \"imageRecipe\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageRecipe\"\n        },\n        {\n          \"description\": \"For images that distribute an AMI, this is the image recipe that Image Builder used to create the image. For container images, this is empty.\"\n        }\n      ]\n    },\n    \"containerRecipe\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerRecipe\"\n        },\n        {\n          \"description\": \"For container images, this is the container recipe that Image Builder used to create the image. For images that distribute an AMI, this is empty.\"\n        }\n      ]\n    },\n    \"sourcePipelineName\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the image pipeline that created this image.\"\n        }\n      ]\n    },\n    \"sourcePipelineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image pipeline that created this image.\"\n        }\n      ]\n    },\n    \"infrastructureConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InfrastructureConfiguration\"\n        },\n        {\n          \"description\": \"The infrastructure that Image Builder used to create this image.\"\n        }\n      ]\n    },\n    \"distributionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DistributionConfiguration\"\n        },\n        {\n          \"description\": \"The distribution configuration that\
  \ Image Builder used to create this image.\"\n        }\n      ]\n    },\n    \"imageTestsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageTestsConfiguration\"\n        },\n        {\n          \"description\": \"The image tests that ran when that Image Builder created this image.\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which Image Builder created this image.\"\n        }\n      ]\n    },\n    \"outputResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputResources\"\n        },\n        {\n          \"description\": \"The output resources that Image Builder produces for this image.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n\
  \          \"description\": \"The tags that apply to this image.\"\n        }\n      ]\n    },\n    \"buildType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildType\"\n        },\n        {\n          \"description\": \"<p>Indicates the type of build that created this image. The build can be initiated in the following ways:</p> <ul> <li> <p> <b>USER_INITIATED</b> \\u2013 A manual pipeline build request.</p> </li> <li> <p> <b>SCHEDULED</b> \\u2013 A pipeline build initiated by a cron expression in the Image Builder pipeline, or from EventBridge.</p> </li> <li> <p> <b>IMPORT</b> \\u2013 A VM import created the image to use as the base image for the recipe.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"imageSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSource\"\n        },\n        {\n          \"description\": \"The origin of the base image that Image Builder used to build this image.\"\n        }\n\
  \      ]\n    },\n    \"scanState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageScanState\"\n        },\n        {\n          \"description\": \"Contains information about the current state of scans for this image.\"\n        }\n      ]\n    },\n    \"imageScanningConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageScanningConfiguration\"\n        },\n        {\n          \"description\": \"Contains settings for vulnerability scans.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: Image
---
