---
description: The image details of the Amazon ECR container image.
layout: schema
name: AwsEcrContainerImageDetails
properties_list:
- description: ''
  name: architecture
  type: object
- description: ''
  name: author
  type: object
- description: ''
  name: imageHash
  type: object
- description: ''
  name: imageTags
  type: object
- description: ''
  name: platform
  type: object
- description: ''
  name: pushedAt
  type: object
- description: ''
  name: registry
  type: object
- description: ''
  name: repositoryName
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-aws-ecr-container-image-details-schema.json
slug: inspector-aws-ecr-container-image-details
source_filename: inspector-aws-ecr-container-image-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aws-ecr-container-image-details-schema.json\",\n  \"title\": \"AwsEcrContainerImageDetails\",\n  \"description\": \"The image details of the Amazon ECR container image.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"architecture\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The architecture of the Amazon ECR container image.\"\n        }\n      ]\n    },\n    \"author\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The image author of the Amazon ECR container image.\"\n        }\n      ]\n    },\n    \"imageHash\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageHash\"\
  \n        },\n        {\n          \"description\": \"The image hash of the Amazon ECR container image.\"\n        }\n      ]\n    },\n    \"imageTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageTagList\"\n        },\n        {\n          \"description\": \"The image tags attached to the Amazon ECR container image.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"The platform of the Amazon ECR container image.\"\n        }\n      ]\n    },\n    \"pushedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeTimestamp\"\n        },\n        {\n          \"description\": \"The date and time the Amazon ECR container image was pushed.\"\n        }\n      ]\n    },\n    \"registry\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n\
  \        },\n        {\n          \"description\": \"The registry for the Amazon ECR container image.\"\n        }\n      ]\n    },\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the repository the Amazon ECR container image resides in.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"imageHash\",\n    \"registry\",\n    \"repositoryName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-aws-ecr-container-image-details-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AwsEcrContainerImageDetails
---
