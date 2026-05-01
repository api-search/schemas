---
description: The defining characteristics of a specific version of an Image Builder image.
layout: schema
name: ImageVersion
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: platform
  type: object
- description: ''
  name: osVersion
  type: object
- description: ''
  name: owner
  type: object
- description: ''
  name: dateCreated
  type: object
- description: ''
  name: buildType
  type: object
- description: ''
  name: imageSource
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-version-schema.json
slug: ec2-image-builder-image-version
source_filename: ec2-image-builder-image-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-version-schema.json\",\n  \"title\": \"ImageVersion\",\n  \"description\": \"The defining characteristics of a specific version of an Image Builder image.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of a specific version of an Image Builder image.</p> <note> <p>Semantic versioning is included in each object's Amazon Resource Name (ARN), at the level that applies to that object as follows:</p> <ol> <li> <p>Versionless ARNs and Name ARNs do not include specific values in any of the nodes. The nodes are either left off entirely, or they are specified as wildcards, for example:\
  \ x.x.x.</p> </li> <li> <p>Version ARNs have only the first three nodes: &lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</p> </li> <li> <p>Build version ARNs have all four nodes, and point to a specific build for a specific version of an object.</p> </li> </ol> </note>\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of this specific version of an Image Builder image.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageType\"\n        },\n        {\n          \"description\": \"Specifies whether this image produces an AMI or a container image.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionNumber\"\n        },\n        {\n          \"description\": \"<p>Details for a specific version of\
  \ an Image Builder image. This version follows the semantic version syntax.</p> <note> <p>The semantic version has four nodes: &lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;/&lt;build&gt;. You can assign values for the first three, and can filter on all of them.</p> <p> <b>Assignment:</b> For the first three nodes you can assign any positive integer value, including zero, with an upper limit of 2^30-1, or 1073741823 for each node. Image Builder automatically assigns the build number to the fourth node.</p> <p> <b>Patterns:</b> You can use any numeric pattern that adheres to the assignment requirements for the nodes that you can assign. For example, you might choose a software version pattern, such as 1.0.0, or a date, such as 2021.01.01.</p> <p> <b>Filtering:</b> With semantic versioning, you have the flexibility to use wildcards (x) to specify the most recent versions or nodes when selecting the base image or components for your recipe. When you use a wildcard in any node, all nodes to the\
  \ right of the first wildcard must also be wildcards.</p> </note>\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"The operating system platform of the image version, for example \\\"Windows\\\" or \\\"Linux\\\".\"\n        }\n      ]\n    },\n    \"osVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OsVersion\"\n        },\n        {\n          \"description\": \"The operating system version of the Amazon EC2 build instance. For example, Amazon Linux 2, Ubuntu 18, or Microsoft Windows Server 2019.\"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The owner of the image version.\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which this specific version of the Image Builder image was created.\"\n        }\n      ]\n    },\n    \"buildType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildType\"\n        },\n        {\n          \"description\": \"<p>Indicates the type of build that created this image. The build can be initiated in the following ways:</p> <ul> <li> <p> <b>USER_INITIATED</b> \\u2013 A manual pipeline build request.</p> </li> <li> <p> <b>SCHEDULED</b> \\u2013 A pipeline build initiated by a cron expression in the Image Builder pipeline, or from EventBridge.</p> </li> <li> <p> <b>IMPORT</b> \\u2013 A VM import created the image to use as the base image for the recipe.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"imageSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSource\"\n        },\n        {\n\
  \          \"description\": \"The origin of the base image that Image Builder used to build this image.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-version-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageVersion
---
