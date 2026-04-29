---
description: ListContainersOutput schema from Amazon MediaStore API
layout: schema
name: ListContainersOutput
properties_list:
- description: ''
  name: Containers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-list-containers-output-schema.json
slug: mediastore-api-list-containers-output
source_filename: mediastore-api-list-containers-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-list-containers-output-schema.json\",\n  \"title\": \"ListContainersOutput\",\n  \"description\": \"ListContainersOutput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Containers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerList\"\n        },\n        {\n          \"description\": \"The names of the containers.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \" <code>NextToken</code> is the token to use in the next call to <code>ListContainers</code>. This token is returned only if you included the <code>MaxResults</code> tag in the original command, and\
  \ only if there are still containers to return. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Containers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-list-containers-output-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListContainersOutput
---
