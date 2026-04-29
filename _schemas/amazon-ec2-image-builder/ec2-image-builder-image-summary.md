---
description: An image summary.
layout: schema
name: ImageSummary
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
  name: state
  type: object
- description: ''
  name: owner
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
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-image-summary-schema.json
slug: ec2-image-builder-image-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-summary-schema.json\",\n  \"title\": \"ImageSummary\",\n  \"description\": \"An image summary.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the image.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageType\"\n        },\n        {\n          \"description\": \"Specifies whether this image\
  \ produces an AMI or a container image.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionNumber\"\n        },\n        {\n          \"description\": \"The version of the image.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"The image operating system platform, such as Linux or Windows.\"\n        }\n      ]\n    },\n    \"osVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OsVersion\"\n        },\n        {\n          \"description\": \"The operating system version of the instances that launch from this image. For example, Amazon Linux 2, Ubuntu 18, or Microsoft Windows Server 2019.\"\n        }\n      ]\n    },\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageState\"\n        },\n\
  \        {\n          \"description\": \"The state of the image.\"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The owner of the image.\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The date on which Image Builder created this image.\"\n        }\n      ]\n    },\n    \"outputResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputResources\"\n        },\n        {\n          \"description\": \"The output resources that Image Builder produced when it created this image.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags\
  \ that apply to this image.\"\n        }\n      ]\n    },\n    \"buildType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildType\"\n        },\n        {\n          \"description\": \"<p>Indicates the type of build that created this image. The build can be initiated in the following ways:</p> <ul> <li> <p> <b>USER_INITIATED</b> \\u2013 A manual pipeline build request.</p> </li> <li> <p> <b>SCHEDULED</b> \\u2013 A pipeline build initiated by a cron expression in the Image Builder pipeline, or from EventBridge.</p> </li> <li> <p> <b>IMPORT</b> \\u2013 A VM import created the image to use as the base image for the recipe.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"imageSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageSource\"\n        },\n        {\n          \"description\": \"The origin of the base image that Image Builder used to build this image.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-image-summary-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ImageSummary
---
