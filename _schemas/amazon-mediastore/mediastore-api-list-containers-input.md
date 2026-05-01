---
description: ListContainersInput schema from Amazon MediaStore API
layout: schema
name: ListContainersInput
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-list-containers-input-schema.json
slug: mediastore-api-list-containers-input
source_filename: mediastore-api-list-containers-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-list-containers-input-schema.json\",\n  \"title\": \"ListContainersInput\",\n  \"description\": \"ListContainersInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Only if you used <code>MaxResults</code> in the first command, enter the token (which was included in the previous response) to obtain the next set of containers. This token is included in a response only if there actually are more containers to list.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerListLimit\"\n        },\n        {\n \
  \         \"description\": \"Enter the maximum number of containers in the response. Use from 1 to 255 characters. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-list-containers-input-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListContainersInput
---
