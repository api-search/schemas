---
description: ListContainerRecipesRequest schema from EC2 Image Builder
layout: schema
name: ListContainerRecipesRequest
properties_list:
- description: ''
  name: owner
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
schema_file: json-schema/ec2-image-builder-list-container-recipes-request-schema.json
slug: ec2-image-builder-list-container-recipes-request
source_filename: ec2-image-builder-list-container-recipes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-container-recipes-request-schema.json\",\n  \"title\": \"ListContainerRecipesRequest\",\n  \"description\": \"ListContainerRecipesRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ownership\"\n        },\n        {\n          \"description\": \"Returns container recipes belonging to the specified owner, that have been shared with you. You can omit this field to return container recipes belonging to your account.\"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterList\"\n        },\n        {\n          \"description\": \"<p>Use the following filters to streamline results:</p>\
  \ <ul> <li> <p> <code>containerType</code> </p> </li> <li> <p> <code>name</code> </p> </li> <li> <p> <code>parentImage</code> </p> </li> <li> <p> <code>platform</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RestrictedInteger\"\n        },\n        {\n          \"description\": \"The maximum items to return in a request.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"A token to specify where to start paginating. This is the NextToken from a previously truncated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-container-recipes-request-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListContainerRecipesRequest
---
