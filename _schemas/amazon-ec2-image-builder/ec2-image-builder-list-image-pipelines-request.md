---
description: ListImagePipelinesRequest schema from EC2 Image Builder
layout: schema
name: ListImagePipelinesRequest
properties_list:
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
schema_file: json-schema/ec2-image-builder-list-image-pipelines-request-schema.json
slug: ec2-image-builder-list-image-pipelines-request
source_filename: ec2-image-builder-list-image-pipelines-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-pipelines-request-schema.json\",\n  \"title\": \"ListImagePipelinesRequest\",\n  \"description\": \"ListImagePipelinesRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterList\"\n        },\n        {\n          \"description\": \"<p>Use the following filters to streamline results:</p> <ul> <li> <p> <code>description</code> </p> </li> <li> <p> <code>distributionConfigurationArn</code> </p> </li> <li> <p> <code>imageRecipeArn</code> </p> </li> <li> <p> <code>infrastructureConfigurationArn</code> </p> </li> <li> <p> <code>name</code> </p> </li> <li> <p> <code>status</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"maxResults\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RestrictedInteger\"\n        },\n        {\n          \"description\": \"The maximum items to return in a request.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A token to specify where to start paginating. This is the NextToken from a previously truncated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-image-pipelines-request-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListImagePipelinesRequest
---
