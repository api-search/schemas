---
description: CreateContainerOutput schema from Amazon MediaStore API
layout: schema
name: CreateContainerOutput
properties_list:
- description: ''
  name: Container
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-create-container-output-schema.json
slug: mediastore-api-create-container-output
source_filename: mediastore-api-create-container-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-create-container-output-schema.json\",\n  \"title\": \"CreateContainerOutput\",\n  \"description\": \"CreateContainerOutput schema from Amazon MediaStore API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Container\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Container\"\n        },\n        {\n          \"description\": \"<p>ContainerARN: The Amazon Resource Name (ARN) of the newly created container. The ARN has the following format: arn:aws:&lt;region&gt;:&lt;account that owns this container&gt;:container/&lt;name of container&gt;. For example: arn:aws:mediastore:us-west-2:111122223333:container/movies </p> <p>ContainerName: The container name as specified in the request.</p> <p>CreationTime: Unix time stamp.</p> <p>Status: The status of container\
  \ creation or deletion. The status is one of the following: <code>CREATING</code>, <code>ACTIVE</code>, or <code>DELETING</code>. While the service is creating the container, the status is <code>CREATING</code>. When an endpoint is available, the status changes to <code>ACTIVE</code>.</p> <p>The return value does not include the container's endpoint. To make downstream requests, you must obtain this value by using <a>DescribeContainer</a> or <a>ListContainers</a>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Container\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-create-container-output-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateContainerOutput
---
