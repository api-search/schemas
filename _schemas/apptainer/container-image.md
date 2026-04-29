---
description: An Apptainer container image (SIF file) for HPC and scientific computing
layout: schema
name: ContainerImage
properties_list:
- description: Unique container image identifier
  name: imageId
  type: string
- description: Container image name
  name: name
  type: string
- description: Container image version
  name: version
  type: string
- description: Source URI (docker://image, library://image, oras://, etc.)
  name: source
  type: string
- description: Container image format
  name: format
  type: string
- description: Image size in bytes
  name: size
  type: integer
- description: Image creation timestamp
  name: createdAt
  type: string
- description: SHA-256 hash of the image for verification
  name: sha256
  type: string
provider_name: Apptainer
provider_slug: apptainer
schema_file: json-schema/container-image-schema.json
slug: container-image
source_filename: container-image-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apptainer/main/json-schema/container-image-schema.json\",\n  \"title\": \"ContainerImage\",\n  \"description\": \"An Apptainer container image (SIF file) for HPC and scientific computing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imageId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique container image identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Container image name\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Container image version\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source URI (docker://image, library://image, oras://, etc.)\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SIF\",\n        \"sandbox\"\n      ],\n      \"description\": \"Container\
  \ image format\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Image size in bytes\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Image creation timestamp\"\n    },\n    \"sha256\": {\n      \"type\": \"string\",\n      \"description\": \"SHA-256 hash of the image for verification\"\n    }\n  },\n  \"required\": [\n    \"imageId\",\n    \"name\",\n    \"format\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apptainer/refs/heads/main/json-schema/container-image-schema.json
tags:
- Containers
- HPC
- Scientific Computing
- Open Source
- Linux Foundation
title: ContainerImage
---
