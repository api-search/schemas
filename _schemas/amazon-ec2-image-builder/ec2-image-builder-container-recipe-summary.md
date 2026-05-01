---
description: A summary of a container recipe
layout: schema
name: ContainerRecipeSummary
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
  name: platform
  type: object
- description: ''
  name: owner
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
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-container-recipe-summary-schema.json
slug: ec2-image-builder-container-recipe-summary
source_filename: ec2-image-builder-container-recipe-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-container-recipe-summary-schema.json\",\n  \"title\": \"ContainerRecipeSummary\",\n  \"description\": \"A summary of a container recipe\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the container recipe.\"\n        }\n      ]\n    },\n    \"containerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerType\"\n        },\n        {\n          \"description\": \"Specifies the type of container, such as \\\"Docker\\\".\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\
  \n        },\n        {\n          \"description\": \"The name of the container recipe.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"The system platform for the container, such as Windows or Linux.\"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The owner of the container recipe.\"\n        }\n      ]\n    },\n    \"parentImage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The base image for the container recipe.\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\"\
  : \"The date when this container recipe was created.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags that are attached to the container recipe.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-container-recipe-summary-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ContainerRecipeSummary
---
