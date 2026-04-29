---
description: CreateImageRecipeRequest schema from EC2 Image Builder
layout: schema
name: CreateImageRecipeRequest
properties_list:
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
  name: parentImage
  type: object
- description: ''
  name: blockDeviceMappings
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
- description: ''
  name: clientToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-create-image-recipe-request-schema.json
slug: ec2-image-builder-create-image-recipe-request
source_filename: ec2-image-builder-create-image-recipe-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-image-recipe-request-schema.json\",\n  \"title\": \"CreateImageRecipeRequest\",\n  \"description\": \"CreateImageRecipeRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the image recipe.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the image recipe.\"\n        }\n      ]\n    },\n    \"semanticVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionNumber\"\
  \n        },\n        {\n          \"description\": \"<p>The semantic version of the image recipe. This version follows the semantic version syntax.</p> <note> <p>The semantic version has four nodes: &lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;/&lt;build&gt;. You can assign values for the first three, and can filter on all of them.</p> <p> <b>Assignment:</b> For the first three nodes you can assign any positive integer value, including zero, with an upper limit of 2^30-1, or 1073741823 for each node. Image Builder automatically assigns the build number to the fourth node.</p> <p> <b>Patterns:</b> You can use any numeric pattern that adheres to the assignment requirements for the nodes that you can assign. For example, you might choose a software version pattern, such as 1.0.0, or a date, such as 2021.01.01.</p> </note>\"\n        }\n      ]\n    },\n    \"components\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentConfigurationList\"\n        },\n \
  \       {\n          \"description\": \"The components included in the image recipe.\"\n        }\n      ]\n    },\n    \"parentImage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The base image of the image recipe. The value of the string can be the ARN of the base image or an AMI ID. The format for the ARN follows this example: <code>arn:aws:imagebuilder:us-west-2:aws:image/windows-server-2016-english-full-base-x86/x.x.x</code>. You can provide the specific version that you want to use, or you can use a wildcard in all of the fields. If you enter an AMI ID for the string value, you must have access to the AMI, and the AMI must be in the same Region in which you are using Image Builder.\"\n        }\n      ]\n    },\n    \"blockDeviceMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceBlockDeviceMappings\"\n        },\n        {\n       \
  \   \"description\": \"The block device mappings of the image recipe.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags of the image recipe.\"\n        }\n      ]\n    },\n    \"workingDirectory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The working directory used during build and test workflows.\"\n        }\n      ]\n    },\n    \"additionalInstanceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdditionalInstanceConfiguration\"\n        },\n        {\n          \"description\": \"Specify additional settings and launch scripts for your build instances.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n\
  \        },\n        {\n          \"description\": \"The idempotency token used to make this request idempotent.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"semanticVersion\",\n    \"components\",\n    \"parentImage\",\n    \"clientToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-create-image-recipe-request-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: CreateImageRecipeRequest
---
