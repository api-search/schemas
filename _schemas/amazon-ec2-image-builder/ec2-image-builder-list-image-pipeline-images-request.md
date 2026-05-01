---
description: ListImagePipelineImagesRequest schema from EC2 Image Builder
layout: schema
name: ListImagePipelineImagesRequest
properties_list:
- description: ''
  name: imagePipelineArn
  type: object
- description: ''
  name: filters
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-list-image-pipeline-images-request-schema.json
slug: ec2-image-builder-list-image-pipeline-images-request
source_filename: ec2-image-builder-list-image-pipeline-images-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-pipeline-images-request-schema.json\",\n  \"title\": \"ListImagePipelineImagesRequest\",\n  \"description\": \"ListImagePipelineImagesRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imagePipelineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImagePipelineArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image pipeline whose images you want to view.\"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterList\"\n        },\n        {\n          \"description\": \"<p>Use the following filters to streamline results:</p> <ul> <li> <p> <code>name</code> </p> </li> <li>\
  \ <p> <code>version</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RestrictedInteger\"\n        },\n        {\n          \"description\": \"The maximum items to return in a request.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A token to specify where to start paginating. This is the NextToken from a previously truncated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"imagePipelineArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-pipeline-images-request-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListImagePipelineImagesRequest
---
