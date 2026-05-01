---
description: ListImagesRequest schema from EC2 Image Builder
layout: schema
name: ListImagesRequest
properties_list:
- description: ''
  name: owner
  type: object
- description: ''
  name: filters
  type: object
- description: ''
  name: byName
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: includeDeprecated
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-list-images-request-schema.json
slug: ec2-image-builder-list-images-request
source_filename: ec2-image-builder-list-images-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-images-request-schema.json\",\n  \"title\": \"ListImagesRequest\",\n  \"description\": \"ListImagesRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ownership\"\n        },\n        {\n          \"description\": \"The owner defines which images you want to list. By default, this request will only show images owned by your account. You can use this field to specify if you want to view images owned by yourself, by Amazon, or those images that have been shared with you by other customers.\"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterList\"\n        },\n        {\n\
  \          \"description\": \"<p>Use the following filters to streamline results:</p> <ul> <li> <p> <code>name</code> </p> </li> <li> <p> <code>osVersion</code> </p> </li> <li> <p> <code>platform</code> </p> </li> <li> <p> <code>type</code> </p> </li> <li> <p> <code>version</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"byName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Requests a list of images with a specific recipe name.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RestrictedInteger\"\n        },\n        {\n          \"description\": \"The maximum items to return in a request.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A token to specify\
  \ where to start paginating. This is the NextToken from a previously truncated response.\"\n        }\n      ]\n    },\n    \"includeDeprecated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"Includes deprecated images in the response list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-images-request-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListImagesRequest
---
