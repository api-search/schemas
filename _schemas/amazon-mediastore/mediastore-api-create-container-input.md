---
description: CreateContainerInput schema from Amazon MediaStore API
layout: schema
name: CreateContainerInput
properties_list:
- description: ''
  name: ContainerName
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-create-container-input-schema.json
slug: mediastore-api-create-container-input
source_filename: mediastore-api-create-container-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-create-container-input-schema.json\",\n  \"title\": \"CreateContainerInput\",\n  \"description\": \"CreateContainerInput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContainerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerName\"\n        },\n        {\n          \"description\": \"The name for the container. The name must be from 1 to 255 characters. Container names must be unique to your AWS account within a specific region. As an example, you could create a container named <code>movies</code> in every region, as long as you don\\u2019t have an existing container with that name.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\
  \n        },\n        {\n          \"description\": \"An array of key:value pairs that you define. These values can be anything that you want. Typically, the tag key represents a category (such as \\\"environment\\\") and the tag value represents a specific value within that category (such as \\\"test,\\\" \\\"development,\\\" or \\\"production\\\"). You can add up to 50 tags to each container. For more information about tagging, including naming and usage conventions, see <a href=\\\"https://docs.aws.amazon.com/mediastore/latest/ug/tagging.html\\\">Tagging Resources in MediaStore</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ContainerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-create-container-input-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateContainerInput
---
